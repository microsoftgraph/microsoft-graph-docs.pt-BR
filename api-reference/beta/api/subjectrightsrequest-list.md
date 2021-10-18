---
title: Listar subjectRightsRequests
description: Obter uma lista de solicitações de direitos de assunto e suas propriedades.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 942eff11c33c38e0cfc9a06ca77efa5d896ec6e3
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447019"
---
# <a name="list-subjectrightsrequests"></a>Listar subjectRightsRequests
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter uma lista de [objetos subjectRightsRequest](../resources/subjectRightsRequest.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|SubjectRightsRequest.Read.All *, SubjectRightsRequest.ReadWrite.All*|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte|

>[!IMPORTANT]
>No momento, as permissões marcadas com um asterisco (*) não estão disponíveis. Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#compliance).

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esse método não dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos subjectRightsRequest](../resources/subjectRightsRequest.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "list_subjectRightsRequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/privacy/subjectRightsRequests
```


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.subjectRightsRequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
        {
    "type": "microsoft.graph.subjectRightsRequestType",
    "dataSubjectType": "microsoft.graph.dataSubjectType",
    "regulations": [
        "String"
    ],
    "displayName": "String",
    "description": "String",
    "status": "active",
    "internalDueDateTime": "String",
    "lastModifiedDateTime": "String",
    "id": "String",
    "createdDateTime": "String",
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
        "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
    },
    "dataSubject": {
        "firstName": "String",
        "lastName": "String",
        "email": "String",
        "residency": "String",
        "phoneNumber": "String",
        "SSN": "String"
    },
    "team": {
        "id": "String (identifier)",
        "webUrl": "String"
    }
    }
  ]
}
```

