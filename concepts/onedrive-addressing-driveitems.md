---
title: Recursos de endereço em uma unidade no OneDrive
description: Saiba como acessar itens em uma unidade no OneDrive com endereçamento baseado em ID e em caminho e como codificar caminhos corretamente para o Microsoft Graph.
ms.localizationpriority: high
ms.prod: sharepoint
author: JeremyKelley
doc_type: conceptualPageType
ms.openlocfilehash: 46f0304dc81245c79213f96cde30efb95766a580
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447118"
---
# <a name="address-resources-in-a-drive-on-onedrive"></a>Recursos de endereço em uma unidade no OneDrive

Saiba como acessar itens em uma unidade no OneDrive com endereçamento baseado em ID e em caminho e como codificar caminhos corretamente para o Microsoft Graph.

## <a name="id-based-addressing"></a>Endereçamento baseado em ID
O OneDrive dá suporte ao endereçamento de itens baseado em ID. Os itens recebem um identificador exclusivo quando são criados, e a ID persiste nas ações que um usuário executa no item. Renomear ou mover o item não mudará a ID do item.

O endereçamento baseado em ID é uma maneira útil de acompanhar itens que podem ser movidos pelo usuário para locais diferentes no OneDrive. Desde que você tenha a ID do item e o item exista, será possível encontrá-lo.

## <a name="path-based-addressing"></a>Endereçamento com base no caminho
O OneDrive também dá suporte ao endereçamento com base no caminho. Isso permite que você use uma sintaxe da URL amigável para endereçar itens em relação à hierarquia de itens visíveis no OneDrive. Se souber a hierarquia de um item, você poderá endereçar diretamente esse item, sem perder tempo fazendo chamadas repetidas para descobrir cada nível da hierarquia.

No entanto, como o endereçamento com base no caminho se baseia no nome do item, renomear ou mover o item para um novo local fará com que o caminho dele seja alterado.

Você pode usar o endereçamento baseado em caminho em relação a qualquer item no OneDrive. Por exemplo, ao trabalhar com pastas compartilhadas, você pode usar uma URL com base em caminho relativa à ID do item da pasta compartilhada para lidar com algo na pasta compartilhada pelo caminho.

## <a name="examples"></a>Exemplos
Os exemplos a seguir mostram os diferentes formatos de URL disponíveis para acessar dados.
Todas essas URLs são logicamente equivalentes e retornam o conteúdo de MyFile.xlsx.

| Exemplo de URL                                       | Descrição                                              |
|:--------------------------------------------------|:---------------------------------------------------------|
| `/drive/root:/Documents/MyFile.xlsx:/content`     | Especificado pelo caminho relativo à raiz de uma unidade.       |
| `/drive/special/documents:/MyFile.xlsx:/content`  | Especificado por filename na pasta especial `documents`. |
| `/drive/items/0123456789AB/content`               | Especificado por item-id.                                    |
| `/drives/AB0987654321/items/0123456789AB/content` | Especificado por drive-id e item-id.                       |


## <a name="path-encoding"></a>Codificação de caminho

O OneDrive suporta o endereçamento de arquivos e pastas usando o caminho do item no OneDrive do usuário. No entanto, como o caminho contém conteúdo especificado pelo usuário, que pode conter potencialmente caracteres que não são seguros para o URL, você deve garantir a codificação adequada de todos os segmentos de caminho.

O Microsoft Graph espera que as URLs estejam em conformidade com [RFC 3986](http://tools.ietf.org/html/rfc3986). A seguir está um resumo de como codificar caminhos corretamente para o Microsoft Graph.

### <a name="onedrive-reserved-characters"></a>Caracteres reservados do OneDrive
Os caracteres a seguir são caracteres reservados do OneDrive e não podem ser usados em nomes de pastas e arquivos do OneDrive.

```
  onedrive-reserved  = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|"
  onedrive-business-reserved
                     = "/" / "\" / "*" / "<" / ">" / "?" / ":" / "|" / "#" / "%"
```

> [!NOTE]
> - Nomes de pastas não podem terminar com um ponto (`.`).
> - Nomes de arquivo ou pasta não podem começar com til (~).
>
> Para mais informações, confira [Restrições e limitações quando você sincronizar as bibliotecas do SharePoint com seu computador por meio do OneDrive para o trabalho ou escola](https://support.microsoft.com/en-us/kb/2933738).

### <a name="uri-path-characters"></a>Caracteres de caminho de URI

Ao construir o segmento de caminho de uma URL para a API do Microsoft Graph, os seguintes caracteres são permitidos para nomes de caminho, com base no RFC do URI.

```
  pchar       = unreserved / pct-encoded / sub-delims / ":" / "@"
  pct-encoded = "%" HEXDIG HEXDIG
  unreserved  = ALPHA / DIGIT / "-" / "." / "_" / "~"
  sub-delims  = "!" / "$" / "&" / "'" / "(" / ")"
              / "*" / "+" / "," / ";" / "="
```

Os caracteres de nome de item, que não são incluídos no grupo `pchar`, como `#` e ` ` (espaço), devem ser codificados como percentual.

### <a name="encoding-characters"></a>Codificação de caracteres
O Microsoft Graph usa a codificação de percentual padrão, em que os caracteres inválidos para URL são codificados com um % e o código de caracteres UTF-8 para o caractere. Por exemplo:

* `" "` -> `%20`
* `"#"` -> `%23`

### <a name="common-url-encoding-mistakes"></a>erros comuns de codificação de URL
Você não pode codificar uma URL inteira em uma chamada, pois as regras de codificação de cada segmento de uma URL são diferentes. Sem codificação adequada, a URL não codificada será ambígua em relação a quais segmentos têm qual conteúdo. Assim, você precisa codificar o caminho da URL durante a criação da cadeia de caracteres de URL.

Por exemplo, em vez de escrever isto:

```
string url = url_encode("https://graph.microsoft.com/v1.0/me/drive/root:/" + path + ":/children")
```

Escreva isto:

```
string url = "https://graph.microsoft.com/v1.0/me/drive/root:/" + url_path_encode(path) + ":/children")
```

No entanto, nem todas as bibliotecas de codificação de URL respeitam todos os requisitos de codificação de caminho de URL padrão.

### <a name="net--c-sharp--visual-basic"></a>.NET/C-Sharp/Visual Basic

As classes .NET para `HttpUtility` e `Uri` incluem vários métodos de codificação de URL. No entanto, nenhum desses métodos codifica corretamente todos os caracteres reservados para o componente de caminho da URL (incluindo `HttpUtility.UrlPathEncode`).

Em vez de usar esses métodos, você deve usar `UriBuilder` para construir uma URL com escape correto.

```csharp
UriBuilder builder = new UriBuilder("https://graph.microsoft.com");
builder.Path = "/v1.0/me/drive/root:/Documents/My Files/#nine.docx";
Uri url = builder.Uri;
```

### <a name="objective-c--ios"></a>Objective-C/iOS

Para o desenvolvimento em Objective-C, iOS e Mac OS X, use o método `stringByAddingPercentEncodingWithAllowedCharacters` e `[NSCharacterSet URLPathAllowedCharacterSet]` para codificar corretamente o componente de caminho da URL.

```objc
NSString *root = @"https://graph.microsoft.com/v1.0/me/drive/root:/";
NSString *path = @"Documents/My Files/#nine.docx";
NSString *encPath = [path stringByAddingPercentEncodingWithAllowedCharacters:[NSCharacterSet URLPathAllowedCharacterSet]];
NSURL *url = [[NSURL alloc] initWithString:[root stringByAppendingString:encPath]];
```


### <a name="android"></a>Android

Use a classe `Uri.Builder` para construir uma URL codificada corretamente.

```java
Uri.Builder builder = new Uri.Builder();
builder.
  scheme("https").
  authority("graph.microsoft.com").
  appendPath("v1.0").
  appendPath("me").
  appendPath("drive").
  appendPath("root:").
  appendPath("Documents").
  appendPath("My Files").
  appendPath("#nine.docx");
String url = builder.build().toString();
```

### <a name="javascript"></a>JavaScript

Use `escape()` em JavaScript para codificar adequadamente um componente de caminho.

```javascript
var root = "https://graph.microsoft.com/v1.0/me/drive/root:";
var path = "/Documents/My Files/#nine.docx";
var url = root + escape(path);
```

### <a name="examples"></a>Exemplos

Aqui está um exemplo de um usuário do OneDrive (Adele) com a seguinte hierarquias de pastas:
```
OneDrive
    \Adele's Files
        \doc (1).docx
    \estimate%s.docx
    \Break#Out
        \saved_game[1].bin
```

Para endereçar cada um dos arquivos de Adele, utilize a codificação percentual, da seguinte forma:

| Caminho                     | URL codificada para caminho                      |
|:-------------------------|:------------------------------------------|
| `\Adele's Files`          | `/root:/Adele's%20Files`                   |
| `\...\doc (1).docx`      | `/root:/Adele's%20Files/doc%20(1).docx`    |
| `\...\estimate%.docx`    | `/root:/Adele's%20Files/estimate%25s.docx` |
| `\Break#Out`             | `/root:/Break%23Out`                      |
| `\...\saved_game[1].bin` | `/root:/Break%23Out/saved_game[1].bin`    |

## <a name="see-also"></a>Confira também

- [Visão geral da API de armazenamento de arquivos do OneDrive](onedrive-concept-overview.md)