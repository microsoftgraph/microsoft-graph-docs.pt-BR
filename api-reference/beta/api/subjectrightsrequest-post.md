---
title: Criar subjectRightsRequest
description: Crie um novo objeto subjectRightsRequest.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9c4530948142d639295993d24f4c44392e647af4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461489"
---
# <a name="create-subjectrightsrequest"></a>Criar subjectRightsRequest
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto subjectRightsRequest](../resources/subjectrightsrequest.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|SubjectRightsRequest.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

[!INCLUDE [subject-rights-request-privacy-deprecate](../../includes/subject-rights-request-privacy-deprecate.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/subjectRightsRequests
POST /privacy/subjectRightsRequests

```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto subjectRightsRequest](../resources/subjectrightsrequest.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [subjectRightsRequest](../resources/subjectrightsrequest.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| contentQuery         | String | KQL consulta de conteúdo baseada em conteúdo que deve ser usada para pesquisa. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|dataSubject|[microsoft.graph.dataSubject](../resources/datasubject.md)|Contém as propriedades do titular dos dados para a solicitação.|
|dataSubjectType|dataSubjectType|Tipo de entidade de dados. Os valores possíveis são: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|String|Descrição da solicitação.|
|displayName|String|Nome da solicitação.|
| externalId           | Cadeia de caracteres| A ID externa da solicitação que é imutável após a criação e é usada para acompanhar a solicitação para o sistema externo. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
| includeAllVersions   | Booliano | Inclua todas as versões dos documentos. Por padrão, as cópias atuais dos documentos serão retornadas. Se SharePoint sites tiverem o controle de versão habilitado, incluir todas as versões incluirá as cópias históricas dos documentos. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
| includeAuthoredContent| Booliano | Inclua o conteúdo criado pelo titular dos dados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|internalDueDateTime|DateTimeOffset|Data de conclusão interna que é usada para acompanhar a conclusão da solicitação.|
| mailboxLocations     | [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)|Os locais de caixa de correio que devem ser pesquisados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
| pauseAfterEstimate   | Booliano| Pause a solicitação após a conclusão da estimativa. Por padrão, a estimativa de dados será executada e pausada, permitindo que você visualize os resultados e selecione a opção para recuperar dados na interface do usuário. Você pode definir essa propriedade como `false` se quiser que ela execute a estimativa e comece automaticamente com a recuperação do conteúdo. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|Regulamentos|Coleção String|Um ou mais regulamentos para a solicitação.|
| siteLocations| [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)| Os SharePoint e OneDrive locais do site que devem ser pesquisados. Essa propriedade é definida somente para APIs acessadas usando `\security` o caminho de consulta e não o `\privacy` caminho da consulta.|
|type|subjectRightsRequestType|Tipo da solicitação. Os valores possíveis são: `export`, `access`, `tagForAction`, `unknownFutureValue`. No `delete` momento, não há suporte para o tipo.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `201 Created` de resposta e um [objeto subjectRightsRequest](../resources/subjectRightsRequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subjectRightsRequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests
Content-Type: application/json

{
    "type": "export",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "dataSubjectType": "customer",
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "includeAllVersions": false,
    "includeAuthoredContent": true,
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "mailboxLocations": null,
    "pauseAfterEstimate": true,
    "regulations": [
        "CCPA"
    ],
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subjectrightsrequest-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subjectrightsrequest-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subjectrightsrequest-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subjectrightsrequest-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subjectRightsRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "type": "export",
    "dataSubjectType": "customer",
    "regulations": [
        "CCPA"
    ],
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "status": "active",
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "lastModifiedDateTime": "2022-05-10T22:42:28Z",
    "id": "CA084038-C5D2-493D-8DAB-23FC12393C76",
    "createdDateTime": "2022-05-10T22:42:28Z",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "contentReview",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": null
        }
    ],
    "createdBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "team": {
        "id": "5484809c-fb5b-415a-afc6-da7ff601034e",
        "webUrl": "https://teams.contoso.com/teams/teamid"
    },
    "includeAllVersions": false,
    "pauseAfterEstimate": false,
    "includeAuthoredContent": false,
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "mailboxLocations": null,
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```

