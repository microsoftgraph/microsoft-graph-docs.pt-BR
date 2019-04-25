---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Acessar itens compartilhados
localization_priority: Normal
ms.openlocfilehash: 1f172060a8b30996ff09b3ca93390da503db9fea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537451"
---
# <a name="accessing-shared-driveitems"></a>Acessar DriveItems compartilhados

Acesse um [DriveItem](../resources/driveitem.md) compartilhado ou uma coleção de itens compartilhados usando um **shareId** ou uma URL de compartilhamento.

Para usar uma URL de compartilhamento com esta API, seu aplicativo precisa [transformar a URL em um token de compartilhamento](#encoding-sharing-urls).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="path-parameters"></a>Parâmetros do caminho

| Nome do Parâmetro                 | Valor    | Descrição                                                                         |
|:-------------------------------|:---------|:------------------------------------------------------------------------------------|
| **shareIdOrEncodedSharingUrl** | `string` | Obrigatório. Um token de compartilhamento retornado pela API ou uma URL de compartilhamento corretamente codificada. |

### <a name="encoding-sharing-urls"></a>Codificação de URLs de compartilhamento

Para codificar uma URL de compartilhamento, use a seguinte lógica:

1. Primeiro, use base64 para codificar a URL.
2. Converta o resultado codificado na base64 para o [formato base64url sem preenchimento](https://en.wikipedia.org/wiki/Base64) removendo caracteres `=` do final do valor, substituindo `/` por `_` e `+` por `-`.)
3. Acrescente `u!` ao início da cadeia de caracteres.

Por exemplo, para codificar uma URL em C#:

```csharp
string sharingUrl = "https://onedrive.live.com/redir?resid=1231244193912!12&authKey=1201919!12921!1";
string base64Value = System.Convert.ToBase64String(System.Text.Encoding.UTF8.GetBytes(sharingUrl));
string encodedUrl = "u!" + base64Value.TrimEnd('=').Replace('/','_').Replace('+','-');
```

## <a name="optional-request-headers"></a>Cabeçalhos de solicitação opcionais

| Nome       | Tipo   | Descrição                                                    |
|:-----------|:-------|:---------------------------------------------------------------|
| **Prefer** | string | Opcional. Defina como um dos `prefer` valores documentados abaixo.  |

### <a name="prefer-header-values"></a>Preferir valores de cabeçalho

| Nome                          | Descrição                                                                                             |
|:------------------------------|:--------------------------------------------------------------------------------------------------------|
| redeemSharingLink             | Se o **shareIdOrEncodedSharingUrl** for um link de compartilhamento, conceda ao chamador acesso durável ao item    |
| redeemSharingLinkIfNecessary  | O mesmo que redeemSharingLink, mas o acesso só é garantido para a duração da solicitação |

redeemSharingLink deve ser considerado equivalente ao chamador navegando para o link de compartilhamento do navegador (aceitando o gesto de compartilhamento), enquanto o redeemSharingLinkIfNecessary se destina a cenários em que a intenção é simplesmente exibir o link do los.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [sharedDriveItem](../resources/shareddriveitem.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação para recuperar um item compartilhado:

<!-- { "blockType": "request", "name": "get-shared-root" } -->

```http
GET /shares/{shareIdOrEncodedSharingUrl}
```

### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.sharedDriveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "B64397C8-07AE-43E4-920E-32BFB4331A5B",
  "name": "contoso project.docx",
  "owner": {
    "user": {
      "id": "98E88F1C-F8DC-47CC-A406-C090248B30E5",
      "displayName": "Ryan Gregg"
    }
  }
}
```

## <a name="access-the-shared-item-directly"></a>Acessar diretamente o item compartilhado

Embora [**SharedDriveItem**](../resources/shareddriveitem.md) contenha algumas informações úteis, a maioria dos aplicativos acessará diretamente o [DriveItem](../resources/driveitem.md) compartilhado. O recurso **SharedDriveItem** inclui **root** e relações **itens** que podem acessar o conteúdo no escopo do item compartilhado.

## <a name="example-single-file"></a>Exemplo (arquivo único)

### <a name="request"></a>Solicitação

Ao solicitar a relação **driveItem**, o **DriveItem** compartilhado será retornado.

<!-- { "blockType": "request", "name": "get-shared-driveitem" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "contoso project.docx",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "file": {},
  "size": 109112
}
```

## <a name="example-shared-folder"></a>Exemplo (pasta compartilhada)

### <a name="request"></a>Solicitação

Solicitando a relação **driveItem** e expandindo a coleção **children**, o **DriveItem** que foi compartilhado será retornado junto com os arquivos da pasta compartilhada.

<!-- { "blockType": "request", "name": "get-shared-driveitem-expand-children" } -->

```http
GET /shares/{shareIdOrUrl}/driveItem?$expand=children
```

### <a name="response"></a>Resposta

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "9FFFDB3C-5B87-4062-9606-1B008CA88E44",
  "name": "Contoso Project",
  "eTag": "2246BD2D-7811-4660-BD0F-1CF36133677B,1",
  "folder": {},
  "size": 10911212,
  "children": [
    {
      "id": "AFBBDD79-868E-452D-AD4D-24697D4A4044",
      "name": "Propsoal.docx",
      "file": {},
      "size": 19001
    },
    {
      "id": "A91FE90A-2F2C-4EE6-B412-C4FFBA3F71A6",
      "name": "Update to Proposal.docx",
      "file": {},
      "size": 91001
    }
  ]
}
```

## <a name="error-responses"></a>Respostas de erro

Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].

## <a name="remarks"></a>Comentários

* Para o OneDrive for Business e o SharePoint, a API Shares sempre requer autenticação e não pode ser usada para acessar conteúdo compartilhado anonimamente sem um contexto de usuário.

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Access the contents of a sharing link with the OneDrive API.",
  "keywords": "shares,shared,sharing,share link, sharing link, share id, share token",
  "section": "documentation",
  "tocPath": "Sharing/Use a link"
} -->
