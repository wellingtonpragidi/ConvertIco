[![GitHub release](https://img.shields.io/github/v/release/wellingtonpragidi/ConvertIco)]()
[![License](https://img.shields.io/github/license/wellingtonpragidi/ConvertIco)]()
# ConvertIco

**README.md (English)**
## Image to ICO converter

A small and straight forward PHP class to convert images into `.ico` files.  
No dependencies, no outdated cruft, no "modern PHP ceremony". Only what matters.

Supported input formats:
- PNG (transparency preserved)
- JPEG / JPG
- GIF
- BMP
- WEBP (transparency preserved)

The converter automatically handles multiple sizes inside the same ICO when desired.

<h3 id="usage">Usage</h3>

#### Example 1 — From Uploaded File (`$_FILES`)

```php

$ico = new ConvertIco( 'file', [32, 32] );
$ico->save( __DIR__ . '/favicon.ico' );
```

#### Example 2 — From Local File Path
```php
$filepath = '/path/to/image.png';
$ico = new ConvertIco( $filepath, [32, 32], false );
$ico->save( __DIR__ . '/favicon.ico' );
```

Notes:
- Built for PHP 8.1+
- No namespaces required unless you want them
- No Composer dependency hell
- Clean, minimal, predictable

---

**README.md (Português)**
## Conversor de Imagem para ICO

Uma classe PHP pequena e direta para converter imagens em arquivos `.ico`.  
Sem dependências externas, sem restos de código dos anos 2000, sem burocracia de framework.

Formatos suportados:
- PNG (mantém transparência)
- JPEG / JPG
- GIF
- BMP
- WEBP (mantém transparência)

O conversor pode gerar arquivos ICO com múltiplos tamanhos quando necessário.

<a href="#usage">Exemplos de uso</a>
