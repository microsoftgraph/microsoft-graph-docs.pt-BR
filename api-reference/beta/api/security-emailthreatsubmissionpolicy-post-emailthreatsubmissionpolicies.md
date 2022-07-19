---
title: Criar emailThreatSubmissionPolicy
description: Crie um novo objeto emailThreatSubmissionPolicy.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 93209290935f35d25e3f349622070aa8dc88b40c
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856500"
---
# <a name="create-emailthreatsubmissionpolicy"></a>Criar emailThreatSubmissionPolicy

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|ThreatSubmissionPolicies.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo|ThreatSubmissionPolicy.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/threatSubmission/emailThreatSubmissionPolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .

Você também pode especificar as propriedades a seguir ao criar um **emailThreatSubmissionPolicy**. Essas propriedades estão relacionadas às configurações de mensagem relatadas pelo usuário. Para obter detalhes, consulte [Configurações de mensagem relatadas pelo usuário](/microsoft-365/security/office-365-security/user-submission.md).

| Propriedade                                 | Tipo    | Descrição                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | Cadeia de caracteres  | Especifica o endereço de email do remetente do qual as notificações por email serão enviadas aos usuários finais para informá-los se um email é spam, phishing ou limpo. O valor padrão é `null`. Opcional para criação.                   |
| customizedReportRecipientEmailAddress    | String  | Especifica o destino em que as mensagens relatadas dos usuários finais chegarão sempre que relatarem algo como phishing, lixo eletrônico ou não. O valor padrão é `null`. Opcional para criação. |
| isAlwaysReportEnabledForUsers            | Booliano | Indica se os usuários finais podem relatar uma mensagem como spam, phishing ou lixo eletrônico diretamente sem uma confirmação (pop-up). O valor padrão é `true`.  Opcional para criação.          |
| isAskMeEnabledForUsers                   | Booliano | Indica se os usuários finais podem confirmar o uso de um pop-up antes de relatar mensagens como spam, phishing ou não lixo eletrônico. O valor padrão é `true`.  Opcional para criação. |
| isCustomizedMessageEnabled               | Booliano | Indica se as notificações por email enviadas aos usuários finais para informá-los se um email é phishing, spam ou lixo eletrônico é personalizado ou não. O valor padrão é `false`. Opcional para criação.                  |
| isCustomizedMessageEnabledForPhishing    | Booliano | Se habilitada, a mensagem personalizada só será exibida quando o email for relatado como phishing. O valor padrão é `false`. Opcional para criação. |
| isCustomizedNotificationSenderEnabled    | Booliano | Indica se o endereço de email do remetente deve ser usado usando customizedNotificationSenderEmailAddress para enviar notificações por email aos usuários finais. O valor padrão é `false`. Opcional para criação.               |
| isNeverReportEnabledForUsers             | Booliano | Indica se os usuários finais podem simplesmente mover a mensagem de uma pasta para outra com base na ação de spam, phishing ou não lixo eletrônico sem realmente reportá-la. O valor padrão é `true`. Opcional para criação.         |
| isOrganizationBrandingEnabled            | Booliano | Indica se o logotipo da identidade visual deve ser usado nas notificações por email enviadas aos usuários finais. O valor padrão é `false`. Opcional para criação.        |
| isReportFromQuarantineEnabled            | Booliano | Indica se os usuários finais podem enviar da página de quarentena. O valor padrão é `true`. Opcional para criação.              |
| isReportToCustomizedEmailAddressEnabled  | Booliano | Indica se os emails relatados pelos usuários finais devem ser enviados para a caixa de correio personalizada configurada usando customizedReportRecipientEmailAddress.  O valor padrão é `false`. Opcional para criação.              |
| isReportToMicrosoftEnabled               | Booliano | Se habilitado, o email será enviado à Microsoft para análise. O valor padrão é `false`. Solicitado para criação.  |
| isReviewEmailNotificationEnabled         | Booliano | Indica se uma notificação por email é enviada ao usuário final que relatou o email quando ele foi revisado pelo administrador. O valor padrão é `false`. Opcional para criação.  |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_emailthreatsubmissionpolicy_from_emailthreatsubmissionpolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/threatSubmission/emailthreatSubmissionPolicies
Content-type: application/json

{
  "isReportToMicrosoftEnabled": true
}
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
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.emailThreatSubmissionPolicy",
  "id": "DefaultReportSubmissionPolicy",
  "isReportToMicrosoftEnabled": true,
  "isReportToCustomizedEmailAddressEnabled": false,
  "isAskMeEnabledForUsers": true,
  "isAlwaysReportEnabledForUsers": true,
  "isNeverReportEnabledForUsers": true,
  "isCustomizedMessageEnabledForPhishing": false,
  "isCustomizedMessageEnabled": false,
  "customizedReportRecipientEmailAddress": null,
  "isReviewEmailNotificationEnabled": false,
  "isCustomNotificationSenderEnabled": false,
  "isOrganizationBrandingEnabled": false,
  "customizedNotificationSenderEmailAddress": null,
  "isReportFromQuarantineEnabled": false
}
```

