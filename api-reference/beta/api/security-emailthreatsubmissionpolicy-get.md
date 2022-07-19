---
title: Obter emailThreatSubmissionPolicy
description: Leia as propriedades e as relações de um objeto emailThreatSubmissionPolicy.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 39d74fc106a9a3911dd421d52ad264354cc38c87
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856471"
---
# <a name="get-emailthreatsubmissionpolicy"></a>Obter emailThreatSubmissionPolicy
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ThreatSubmission.Read, ThreatSubmission.ReadWrite, ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All, ThreatSubmissionPolicies.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|ThreatSubmission.Read.All, ThreatSubmission.ReadWrite.All, ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET security/threatSubmission//emailThreatSubmissionPolicies/{emailThreatSubmissionPoliciesId}
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

Se tiver êxito, este método retornará um `200 OK` código de resposta e um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "get_emailthreatsubmissionpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/threatSubmission/emailThreatSubmissionPolicies/{emailThreatSubmissionPoliciesId}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.emailThreatSubmissionPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
    "id": "3df67ecc-11b4-b5b4-9bae-b0729940b3d1",
    "isReportToMicrosoftEnabled": "Boolean",
    "isReportToCustomizedEmailAddressEnabled": "Boolean",
    "isAskMeEnabledForUsers": "Boolean",
    "isAlwaysReportEnabledForUsers": "Boolean",
    "isNeverReportEnabledForUsers": "Boolean",
    "isCustomizedMessageEnabledForPhishing": "Boolean",
    "isCustomizedMessageEnabled": "Boolean",
    "customizedReportRecipientEmailAddress": "String",
    "isReviewEmailNotificationEnabled": "Boolean",
    "isCustomizedNotificationSenderEnabled": "Boolean",
    "isOrganizationBrandingEnabled": "Boolean",
    "customizedNotificationSenderEmailAddress": "String",
    "isReportFromQuarantineEnabled": "Boolean"
  }
}
```

