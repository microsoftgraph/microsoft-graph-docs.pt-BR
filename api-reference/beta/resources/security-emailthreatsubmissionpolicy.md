---
title: Tipo de recurso emailThreatSubmissionPolicy
description: Representa as diretrizes de uma organização para relatar possíveis ameaças e spam.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d34e239e9c7717aaf21d2619a47ab3a005b42d7b
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856567"
---
# <a name="emailthreatsubmissionpolicy-resource-type"></a>Tipo de recurso emailThreatSubmissionPolicy

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as diretrizes de uma organização para relatar possíveis ameaças e mensagens de spam. Ele é usado para personalizar a experiência de envio de ameaças do usuário final da sua organização ao relatar possíveis ameaças e spam no Microsoft Outlook.


Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar emailThreatSubmissionPolicies](../api/security-emailthreatsubmissionpolicy-list.md)|[coleção microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Obtenha uma lista dos [objetos emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) e suas propriedades.|
|[Criar emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-post-emailthreatsubmissionpolicies.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Crie um novo [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Obter emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-get.md)|[microsoft.graph.security.emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md)|Leia as propriedades e as relações de um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Atualizar emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-update.md)|Nenhum|Atualize as propriedades de um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|
|[Excluir emailThreatSubmissionPolicy](../api/security-emailthreatsubmissionpolicy-delete.md)|Nenhum|Exclui um [objeto emailThreatSubmissionPolicy](../resources/security-emailthreatsubmissionpolicy.md) .|

## <a name="properties"></a>Propriedades
| Propriedade                                 | Tipo    | Descrição                                                                                |
|:-----------------------------------------|:--------|:-------------------------------------------------------------------------------------------|
| customizedNotificationSenderEmailAddress | Cadeia de caracteres  | Especifica o endereço de email do remetente do qual as notificações por email serão enviadas aos usuários finais para informá-los se um email é spam, phishing ou limpo. O valor padrão é `null`. Opcional para criação.                   |
| customizedReportRecipientEmailAddress    | String  | Especifica o destino em que as mensagens relatadas dos usuários finais chegarão sempre que relatarem algo como phishing, lixo eletrônico ou não. O valor padrão é `null`. Opcional para criação. |
| id                                       | Cadeia de caracteres  | Há suporte para apenas uma ID. O valor padrão é `DefaultReportSubmissionPolicy`. |
| isAlwaysReportEnabledForUsers            | Booliano | Indica se os usuários finais podem relatar uma mensagem como spam, phishing ou lixo eletrônico diretamente sem uma confirmação (pop-up). O valor padrão é `true`.  Opcional para criação.          |
| isAskMeEnabledForUsers                   | Booliano | Indica se os usuários finais podem confirmar o uso de um pop-up antes de relatar mensagens como spam, phishing ou não lixo eletrônico. O valor padrão é `true`.  Opcional para criação.   |
| isCustomizedMessageEnabled               | Booliano | Indica se as notificações por email enviadas aos usuários finais para informá-los se um email é phishing, spam ou lixo eletrônico é personalizado ou não. O valor padrão é `false`. Opcional para criação.    |
| isCustomizedMessageEnabledForPhishing    | Booliano | Se habilitada, a mensagem personalizada só será exibida quando o email for relatado como phishing. O valor padrão é `false`. Opcional para criação. |
| isCustomizedNotificationSenderEnabled    | Booliano | Indica se o endereço de email do remetente deve ser usado usando customizedNotificationSenderEmailAddress para enviar notificações por email aos usuários finais. O valor padrão é `false`. Opcional para criação.  |
| isNeverReportEnabledForUsers             | Booliano | Indica se os usuários finais podem simplesmente mover a mensagem de uma pasta para outra com base na ação de spam, phishing ou não lixo eletrônico sem realmente reportá-la. O valor padrão é `true`. Opcional para criação.         |
| isOrganizationBrandingEnabled            | Booliano | Indica se o logotipo da identidade visual deve ser usado nas notificações por email enviadas aos usuários finais. O valor padrão é `false`. Opcional para criação.        |
| isReportFromQuarantineEnabled            | Booliano | Indica se os usuários finais podem enviar da página de quarentena. O valor padrão é `true`. Opcional para criação.  |
| isReportToCustomizedEmailAddressEnabled  | Booliano | Indica se os emails relatados pelos usuários finais devem ser enviados para a caixa de correio personalizada configurada usando customizedReportRecipientEmailAddress.  O valor padrão é `false`. Opcional para criação.              |
| isReportToMicrosoftEnabled               | Booliano | Se habilitado, o email será enviado à Microsoft para análise. O valor padrão é `false`. Necessário para a criação.  |
| isReviewEmailNotificationEnabled         | Booliano | Indica se uma notificação por email é enviada ao usuário final que relatou o email quando ele foi revisado pelo administrador. O valor padrão é `false`. Opcional para criação.  |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmissionPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmissionPolicy",
  "id": "String (identifier)",
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
```

