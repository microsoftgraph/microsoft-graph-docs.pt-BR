---
title: Obter emailThreatSubmission
description: Leia as propriedades e as relações de um objeto emailThreatSubmission.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 0520c991af594a97964c3f9e35a69b09a28d87ac
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856473"
---
# <a name="get-emailthreatsubmission"></a>Obter emailThreatSubmission
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto emailThreatSubmission](../resources/security-emailthreatsubmission.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ThreatSubmission.Read, ThreatSubmission.ReadWrite, ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/threatSubmission/emailThreats/{emailThreatsId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Não suppported.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um [objeto emailThreatSubmission](../resources/security-emailthreatsubmission.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_emailthreatsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/emailThreats/{emailThreatsId}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.emailThreatSubmission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/threatSubmission/emailThreatSubmission/$entity",
  "@odata.type": "#microsoft.graph.emailUrlThreatSubmission",
  "category": "spam",
  "recipientEmailAddress": "tifc@a830edad9050849EQTPWBJZXODQ.onmicrosoft.com",
  "id": "49c5ef5b-1f65-444a-e6b9-08d772ea2059",
  "createdDateTime": "2021-10-10T03:30:18.6890937Z",
  "contentType": "email",
  "emailSubject": "This is a spam",
  "status": "succeeded",
  "source": "administrator",
  "createdBy": {
    "user": {
      "identity": "c52ce8db-3e4b-4181-93c4-7d6b6bffaf60",
      "displayName": "Ronald Admin",
      "email": "tifc@a830edad9050849eqtpwbjzxodq.onmicrosoft.com"
    }
  },
  "result": {
    "detail": "allowedByTenant",
    "category": "notSpam",
    "userMailboxSetting": "isFromDomainInDomainSafeList,isJunkMailRuleEnabled",
    "detectedUrls": ["contoso.com"],
    "detectedFiles": [
        {
            "fileName": "test.ps1",
            "fileHash": "hash of test.ps1"
        }
    ]
  },
  "adminReview": null,
  "internetMessageId": "some-internet-message-id@contoso.com",
  "sender": "test@contoso.com",
  "senderIP": "127.0.0.1",
  "receivedDateTime": "2021-10-09T03:30:18.6890937Z",
  "originalCategory": "notSpam",
  "attackSimulationInfo": null,
  "tenantAllowOrBlockListAction": 
  {
    "action": "allow",
    "expirationDateTime": "2021-10-30T03:30:18.6890937Z",
    "note": "temporal allow the url/attachment/sender in the email.",
    "results": null
  },
  "tenantId" : "39238e87-b5ab-4ef6-a559-af54c6b07b42"
}
```

