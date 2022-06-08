---
title: 'ediscoveryReviewSetQuery: executar'
description: Execute a consulta de conjunto de revisão para obter a lista de arquivos.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7cd479bf477317a410e1ffe7b43f0fc721873270
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945232"
---
# <a name="ediscoveryreviewsetquery-run"></a>ediscoveryReviewSetQuery: executar
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Execute a consulta de conjunto de revisão para obter a lista de arquivos.

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries/{queryId}/run
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma [coleção microsoft.graph.security.ediscoveryFile](../resources/security-ediscoveryfile.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "ediscoveryreviewsetquerythis.run"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/837335b0-1943-444d-a3d1-5522cc21c5a4/run
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(ediscoveryFile)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries/837335b0-1943-444d-a3d1-5522cc21c5a4/run?$top=2&$skiptoken=1",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryFile",
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
        },
        {
            "@odata.type": "#microsoft.graph.security.ediscoveryFile",
            "id": "005248e12e3f4859c8b20f385f7e962f41eeea144cf27baefd339bd5fa8ed39a",
            "dateTime": "2017-10-04T22:42:49Z",
            "size": 19811608,
            "name": "Introducing the Contoso Mark 8 3D.pptx",
            "sourceType": "site",
            "subjectTitle": "PowerPoint Presentation",
            "extension": "pptx",
            "mediaType": "application/vnd.openxmlformats-officedocument.presentationml.presentation",
            "processingStatus": "success",
            "otherProperties": {
                "Source": null,
                "Participants": null,
                "To": null,
                "Cc": null,
                "Bcc": null,
                "Recipients": null,
                "Author@odata.type": "#Collection(String)",
                "Author": [
                    "meganb@m365x809305.onmicrosoft.com"
                ],
                "CreatedTime": "2021-09-14T12:00:53Z",
                "Received": null,
                "Sent": null,
                "LastModifiedDate": "2017-10-04T22:42:49Z",
                "MessageType": null,
                "Title": "PowerPoint Presentation",
                "EmailHasAttachment": false,
                "EmailImportance": "",
                "WordCount": 293,
                "ErrorIgnored": false,
                "IsFromErrorRemediation": false,
                "EmailSecurity": 0,
                "EmailSensitivity": 0,
                "IsModernAttachment": false,
                "IsEmbeddedDocument": false,
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

