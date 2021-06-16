---
author: JeremyKelley
description: Você pode usar a ação createLink para compartilhar um DriveItem por meio de um link de compartilhamento.
title: 'driveItem: createLink'
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a6f3c172efdec9decf2f054a8afbb8d7ccf53034
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941470"
---
# <a name="driveitem-createlink"></a>driveItem: createLink

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar a ação **createLink** para compartilhar um [DriveItem](../resources/driveitem.md) por meio de um link de compartilhamento.

A ação **createLink** criará um novo link de compartilhamento se o tipo de link especificado não existir para o aplicativo de chamada. Se um link de compartilhamento do tipo especificado já existir para o aplicativo, o link de compartilhamento existente será retornado.

Recursos de DriveItem herdam permissões de compartilhamento de seus ancestrais.

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
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

O corpo da solicitação define as propriedades do link de compartilhamento que seu aplicativo está solicitando.
A solicitação deve ser um objeto JSON com as seguintes propriedades.

|   Propriedade                 |  Tipo  |                                 Descrição                                                               |
| :----------------------| :----- | :---------------------------------------------------------------------------------------------------------|
|tipo|Cadeia de caracteres|Optional.O tipo de link de compartilhamento a ser criado.   |
|escopo|String|Opcional. O escopo do link a ser criado. Anônimos, organização ou usuários.|
|expirationDateTime|DateTimeOffset|Opcional. Uma cadeia de caracteres com formato de yyyy-MM-ddTHH:mm:ssZ de DateTime indica o tempo de expiração da permissão.|
|password|String|Optional.A senha do link de compartilhamento que é definido pelo criador.|
|destinatários|[Coleção driveRecipient](../resources/driverecipient.md)|Opcional. Uma coleção de destinatários que receberão acesso ao link de compartilhamento.|

### <a name="link-types"></a>Tipos de link

Os seguintes valores são permitidos para o parâmetro **type**.

| Valor do tipo | Descrição                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| modo de exibição           | Cria um link somente leitura para o Item.                                                                        |
| review         | Cria um link de revisão para o Item. Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.                   |
| edit           | Cria um link de leitura-gravação para o Item.                                                                       |
| Incorporar          | Cria um link inbeddable para o Item.                                                                      |
| blocksDownload | Cria um link somente leitura que bloqueia o download para o Item. Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.  |
| createOnly     | Cria um link somente carregamento para o Item. Essa opção só está disponível para pastas em OneDrive for Business e SharePoint.             |
| addressBar     | Cria o link padrão mostrado nas barras de endereço do navegador para arquivos recém-criados. Disponível apenas no OneDrive for Business e no SharePoint. O administrador da organização configura se esse tipo de link tem suporte e quais recursos são suportados por esse tipo de link. |
| adminDefault   | Cria o link padrão para o DriveItem conforme determinado pelo administrador da organização. Disponível apenas no OneDrive for Business e no SharePoint. A política é imposta para a organização pelo administrador |

### <a name="scope-types"></a>Tipos de escopo

Os seguintes valores são permitidos para o parâmetro **scope**.

| Valor          | Descrição
|:---------------|:------------------------------------------------------------
| anonymous    | Qualquer pessoa com o link tem acesso, sem precisar fazer logon. Isso pode incluir pessoas de fora da organização. O suporte para links anônimos pode ser desativado por um administrador.
| organization | Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.
| usuários        | Pessoas específicas no conjunto de destinatários podem usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.

## <a name="response"></a>Resposta

Se for bem-sucedido, esse método retornará um único recurso [Permission](../resources/permission.md) no corpo da resposta, que representa as permissões de compartilhamento solicitadas.

A resposta será `201 Created` se um novo link de compartilhamento for criado para o item ou `200 OK` se um link existente for retornado.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-an-anonymous-sharing-link"></a>Exemplo 1: Criar um link de compartilhamento anônimo
O exemplo a seguir solicita um link de compartilhamento que será criado para o DriveItem especificado por {itemId} no OneDrive do usuário.
O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "driveItem_createlink",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-Type: application/json
Content-length: 212

{
  "type": "view",
  "scope": "anonymous",
  "password": "String",
  "recipients": [
    {
      "@odata.type": "microsoft.graph.driveRecipient"
    }
  ]
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/item-createlink-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/item-createlink-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/item-createlink-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/item-createlink-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  },
  "hasPassword": true
}
```

### <a name="example-2-creating-company-sharable-links"></a>Exemplo 2: Criação de links compartilháveis da empresa

O OneDrive for Business e o SharePoint oferecem suporte a links compartilháveis pela empresa.
Estes são semelhantes a links anônimos, com a diferença de que apenas funcionam para membros da organização proprietária.
Para criar um link compartilhável pela empresa, use o parâmetro **scope** com um valor de `organization`.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create-link-scoped",
  "scopes": "files.readwrite service.sharepoint",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
 } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

### <a name="example-3-creating-embeddable-links"></a>Exemplo 3: Criação de links inbeddáveis

Ao usar o tipo de link `embed`, a webUrl retornada pode ser inserida em um elemento HTML `<iframe>`. Quando um link de inserção é criado, a propriedade `webHtml` contém o código HTML de um `<iframe>` para hospedar o conteúdo.

>**Observação:** os links de inseridos só tem suporte no OneDrive Pessoal.

#### <a name="request"></a>Solicitar

<!-- {
  "blockType": "request",
  "name": "create-embedded-link",
  "scopes": "files.readwrite service.onedrive",
  "sampleKeys": ["01G7ZEPNWQ6DTNTJHHJFBYZD47OAVFOO46"]
} -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>Comentários

* Para criar um link com base na política padrão da organização e nas permissões do chamador no listItem, omita os parâmetros de escopo e de tipo
* Links criados usando esta ação não expiram, a menos que uma política de expiração padrão seja imposta à organização.
* Os links ficam visíveis nas permissões de compartilhamento do item e podem ser removidos por um proprietário desse item.
* Os links sempre apontam para a versão atual de um item, a menos que esse item esteja em check-out (apenas no SharePoint).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->