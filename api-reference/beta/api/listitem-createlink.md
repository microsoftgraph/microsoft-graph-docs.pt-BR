---
title: 'listItem: createLink'
description: Criar um link para compartilhar um listItem
author: learafa
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b0d490139763e619a151e3152868f98c1f1b96e4
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941575"
---
# <a name="listitem-createlink"></a>listItem: createLink

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um link de compartilhamento para [um listItem](../resources/listitem.md).

A **ação createLink** criará um novo link de compartilhamento se o tipo de link especificado ainda não existir para o aplicativo de chamada.
Se um link de compartilhamento do tipo especificado já existir para o aplicativo, essa ação retornará o link de compartilhamento existente.

**os recursos listItem** herdam permissões de compartilhamento da [lista](../resources/list.md) em que o item reside.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é necessária para chamar essa API. Para saber mais, incluindo como escolher permissões, consulte [permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|   Propriedade             |  Tipo  |           Descrição                        |
| :----------------------| :----- | :--------------------------------------------|
|tipo|String|O tipo de link de compartilhamento a ser criado. Opcional. |
|escopo|String|O escopo do link a ser criado. Ou `anonymous` `organization` `users` . Opcional. |
|expirationDateTime|DateTimeOffset|Uma cadeia de caracteres com formato de yyyy-MM-ddTHH:mm:ssZ de DateTime indica o tempo de expiração da permissão. Opcional. |
|password|String|A senha do link de compartilhamento definido pelo criador. Opcional. |
|destinatários|[Coleção driveRecipient](../resources/driverecipient.md)|Uma coleção de destinatários que receberão acesso ao link de compartilhamento. Opcional. |

### <a name="link-types"></a>Tipos de link

Os seguintes valores são permitidos para o parâmetro **type**.

| Valor do tipo | Descrição                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| modo de exibição           | Cria um link somente leitura para o item.                                                                        |
| review         | Cria um link de revisão para o item. Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.                   |
| edit           | Cria um link de leitura-gravação para o item.                                                                       |
| Incorporar          | Cria um link inserível para o item.                                                                      |
| blocksDownload | Cria um link somente leitura que bloqueia o download para o item. Essa opção só está disponível para arquivos em OneDrive for Business e SharePoint.  |
| createOnly     | Cria um link somente carregamento para o item. Essa opção só está disponível para pastas em OneDrive for Business e SharePoint.             |
| addressBar     | Cria o link padrão mostrado nas barras de endereço do navegador para arquivos recém-criados. Disponível apenas no OneDrive for Business e no SharePoint. O administrador da organização configura se esse tipo de link tem suporte e quais recursos são suportados por esse tipo de link. |
| adminDefault   | Cria o link padrão para o item conforme determinado pelo administrador da organização. Disponível apenas no OneDrive for Business e no SharePoint. A política é imposta para a organização pelo administrador |

### <a name="scope-types"></a>Tipos de escopo

Os seguintes valores são permitidos para o parâmetro **scope**.

| Valor          | Descrição
|:---------------|:------------------------------------------------------------
| anonymous    | Qualquer pessoa com o link tem acesso, sem precisar fazer logon. Isso pode incluir pessoas de fora da organização. O suporte para links anônimos pode ser desativado por um administrador.
| organization | Qualquer pessoa que tenha feito logon em sua organização (locatário) pode usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.
| usuários        | Pessoas específicas no conjunto de destinatários podem usar o link para obter acesso. Disponível apenas no OneDrive for Business e no SharePoint.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um [único](../resources/permission.md) recurso de permissão no corpo da resposta que representa as permissões de compartilhamento solicitadas.

A resposta será `201 Created` se um novo link de compartilhamento for criado para o listItem ou se um link existente for `200 OK` retornado.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-an-anonymous-sharing-link"></a>Exemplo 1: Criar um link de compartilhamento anônimo
O exemplo a seguir solicita que um link de compartilhamento seja criado para o listItem especificado por {itemId} na lista especificada {listId}.
O link de compartilhamento é configurado como somente leitura e utilizável por qualquer pessoa com o link.

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST sites/{siteId}/lists/{listId}/items/{itemId}/createLink
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

#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
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
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

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
  "name": "listItem_createlink",
  "sampleKeys": ["contoso.sharepoint.com,2288913C-B09C-46C4-BD1D-AEBB3A6E08EB,133A857A-DC2E-4A41-BCF7-D2B9BBC016AF", "A90E03FB-8446-4E0F-82E7-810FA7595A66", "3"]
}-->

```http
POST /sites/{siteId}/lists/{listId}/items/{itemId}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

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
* Os links ficam visíveis nas permissões de compartilhamento do listItem e podem ser removidos por um proprietário do listItem.
* Os links sempre apontam para a versão atual de um listItem, a menos que listItem esteja com check-out (SharePoint somente).

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an listItem.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
}
-->