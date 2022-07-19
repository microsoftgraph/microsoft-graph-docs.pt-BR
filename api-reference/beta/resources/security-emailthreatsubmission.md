---
title: Tipo de recurso emailThreatSubmission
description: Relata emails suspeitos de spam, malware ou phishing para Microsoft Defender para Office 365.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 387d4531a6f2e4d4b9184e4006ae43ddac4c15ed
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856506"
---
# <a name="emailthreatsubmission-resource-type"></a>Tipo de recurso emailThreatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo abstrato para relatar emails suspeitos de spam, malware ou phishing para Microsoft Defender para Office 365. Você também pode enviar casos falsos positivos, que não devem ter sido bloqueados por Microsoft Defender para Office 365, por exemplo, emails categorizados incorretamente como lixo eletrônico ou spam.

Herda de [threatSubmission](../resources/security-threatsubmission.md). Tipo base de [emailContentThreatSubmission](../resources/security-emailcontentthreatsubmission.md) e [emailUrlThreatSubmission](../resources/security-emailurlthreatsubmission.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar emailThreatSubmissions](../api/security-emailthreatsubmission-list.md)|[coleção microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Obtenha uma lista dos [objetos emailThreatSubmission](../resources/security-emailthreatsubmission.md) e suas propriedades.|
|[Criar emailThreatSubmission](../api/security-emailthreatsubmission-post-emailthreats.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Crie um novo [objeto emailThreatSubmission](../resources/security-emailthreatsubmission.md) .|
|[Obter emailThreatSubmission](../api/security-emailthreatsubmission-get.md)|[microsoft.graph.security.emailThreatSubmission](../resources/security-emailthreatsubmission.md)|Leia as propriedades e as relações de um [objeto emailThreatSubmission](../resources/security-emailthreatsubmission.md) .|
|[Revisão](../api/security-emailthreatsubmission-review.md)|Nenhum|Examine o envio de ameaças do usuário final por administrador.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo    | Descrição    |
|:-----------------------------|:-----------------------------|:-------------------------------------------------------------------------------------------------------|
| attackSimulationInfo         | [security.attackSimulationInfo](../resources/security-attacksimulationinfo.md) | Se o email for uma simulação de phishing, esse campo não será nulo.|
| internetMessageId            | String                       | Especifica a ID da mensagem da Internet do email que está sendo enviado. Essas informações estão presentes no cabeçalho do email. |
| originalCategory             | submissionCategory           | A categoria original do envio. Os valores possíveis são: `notJunk`, `spam`, `phishing`e `unkownFutureValue``malware` . |
| receivedDateTime             | DateTimeOffset               | Especifica a data e o carimbo de data/hora em que o email foi recebido.  | 
| recipientEmailAddress        | Cadeia de caracteres                       | Especifica o endereço de email (no formato smtp) do destinatário que recebeu o email. |
| sender                       | String                       | Especifica o endereço de email do remetente. | 
| senderIP                     | String                       | Especifica o endereço IP do remetente. |
| assunto                      | Cadeia de caracteres                       | Especifica o assunto do email. |
| tenantAllowOrBlockListAction | [security.tenantAllowOrBlockListAction](../resources/security-tenantalloworblocklistaction.md) | Ele é usado para adicionar automaticamente permissões para os componentes, como URL, arquivo, remetente; que são consideradas ruins pela Microsoft para que mensagens semelhantes no futuro possam ser permitidas. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.emailThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.emailThreatSubmission",
  "id": "String (identifier)",
  "tenantId": "String",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "category": "String",
  "source": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.security.submissionUserIdentity"
  },
  "status": "String",
  "result": {
    "@odata.type": "microsoft.graph.security.submissionResult"
  },
  "adminReview": {
    "@odata.type": "microsoft.graph.security.submissionAdminReview"
  },
  "clientSource": "String",
  "recipientEmailAddress": "String",
  "internetMessageId": "String",
  "subject": "String",
  "sender": "String",
  "senderIP": "String",
  "receivedDateTime": "String (timestamp)",
  "originalCategory": "String",
  "attackSimulationInfo": {
    "@odata.type": "microsoft.graph.security.attackSimulationInfo"
  },
  "tenantAllowOrBlockListAction": {
    "@odata.type": "microsoft.graph.security.tenantAllowOrBlockListAction"
  }
}
```

