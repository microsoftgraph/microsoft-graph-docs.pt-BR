---
title: Listar ediscoveryFiles
description: Obtenha uma lista dos objetos ediscoveryFile e suas propriedades.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9cca478ef643fd799a2dcc34334cf6abe3a43e06
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945235"
---
# <a name="list-ediscoveryfiles"></a>Listar ediscoveryFiles
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obtenha uma lista dos [objetos ediscoveryFile](../resources/security-ediscoveryfile.md) e suas propriedades.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e uma coleção [de objetos ediscoveryFile](../resources/security-ediscoveryfile.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5
```


### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryFile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/files",
    "@odata.nextLink": "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5&$skiptoken=1",
    "value": [
        {
            "id": "000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661",
            "dateTime": "2017-11-02T15:07:10Z",
            "size": 921,
            "name": "Report/CustomVisuals/WordCloud1447959067750/package.json",
            "sourceType": "site",
            "subjectTitle": "Operations Analytics.pbix",
            "extension": "json",
            "mediaType": "application/json; charset=ISO-8859-1",
            "processingStatus": "success",
            "otherProperties": {
                "Source": null,
                "Participants": null,
                "To": null,
                "Cc": null,
                "Bcc": null,
                "Recipients": null,
                "Author": null,
                "CreatedTime": null,
                "Received": null,
                "Sent": null,
                "LastModifiedDate": "2017-11-02T15:07:10Z",
                "MessageType": null,
                "Title": null,
                "EmailHasAttachment": false,
                "EmailImportance": "",
                "WordCount": 25,
                "ErrorIgnored": false,
                "IsFromErrorRemediation": false,
                "EmailSecurity": 0,
                "EmailSensitivity": 0,
                "IsModernAttachment": false,
                "IsEmbeddedDocument": true,
                "ComplianceLabels": null,
                "ConversationId": null,
                "ConversationIndex": null,
                "ItemClass": null,
                "LocationName": null,
                "MeetingStartDate": null,
                "MeetingEndDate": null,
                "ParticipantDomains": null,
                "RecipientDomains": null,
                "Sender": null,
                "SenderDomain": null
            }
        }
    ]
}
```

