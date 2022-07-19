---
title: Tipo de recurso threatSubmission
description: Representa um envio de ameaças, que é usado para enviar emails, UTL ou ameaças de arquivo suspeitos ao Microsoft Defender.
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23651a4b66c68ce1c8d128268dd786dfcf667cf8
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856503"
---
# <a name="threatsubmission-resource-type"></a>Tipo de recurso threatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um envio de ameaças, que é um tipo abstrato para representar spam, malware, phishing e emails legítimos bloqueados suspeitos; malware, phishing e URLs legítimas bloqueadas; phish, malware e anexos de email legítimos bloqueados para Microsoft Defender para Office 365 e arquivos suspeitos para Microsoft Defender para Ponto de Extremidade.

Esse recurso também pode ser usado para enviar casos falsos positivos que não devem ser bloqueados pelo Microsoft Defender para Office 365; por exemplo, não emails de lixo eletrônico, URLs seguras e anexos de email seguros.

Esse é um tipo abstrato. Herda de [entidade](../resources/entity.md). Tipo base de [emailThreatSubmission](../resources/security-emailthreatsubmission.md), [urlThreatSubmission](../resources/security-urlthreatsubmission.md), [fileThreatSubmissin](../resources/security-filethreatsubmission.md).

## <a name="properties"></a>Propriedades
| Propriedade        | Tipo                       | Descrição                                                                      |
|:----------------|:---------------------------|:---------------------------------------------------------------------------------|
| adminReview     | [security.submissionAdminReview](../resources/security-submissionadminreview.md)| Especifica a propriedade de revisão do administrador que constitui quem examinou o envio do usuário, quando e o que foi identificado como. |
| category        | submissionCategory         | Especifica a categoria do envio. Oferece suporte para `$filter = category eq 'value'`. Os valores possíveis são: `notJunk`, `spam`, `phishing`e `unkownFutureValue``malware` .|
| clientSource    | submissionClientSource     | Especifica a origem do envio. Os valores possíveis são: `microsoft`e `unkownFutureValue``other` . |
| contentType     | submissionContentType      | Especifica o tipo de conteúdo que está sendo enviado. Os valores possíveis são: `email`, `url`, `file`e `unkownFutureValue``app` .  |
| createdBy       | [security.submissionUserIdentity](../resources/security-submissionuseridentity.md)     | Especifica quem enviou o email como uma ameaça. Oferece suporte para `$filter = createdBy/email eq 'value'`. |
| createdDateTime | DateTimeOffset  | Especifica quando o envio de ameaças foi criado. Oferece suporte para `$filter = createdDateTime ge 2022-01-01T00:00:00Z and createdDateTime lt 2022-01-02T00:00:00Z`.             |
| id              | Cadeia de caracteres                     | Especifica a ID do envio de ameaças. |
| resultado          | [security.submissionResult](../resources/security-submissionresult.md)          | Especifica o resultado da análise executada pela Microsoft.  |
| source          | submissionSource           | Especifica a função do enviador. Oferece suporte para `$filter = source eq 'value'`. Os valores possíveis são: `administrator`e `unkownFutureValue``user` .  |
| status          | Longrunningoperationstatus | Indica se o envio de ameaças foi analisado pela Microsoft. Oferece suporte para `$filter = status eq 'value'`. Os valores possíveis são: `notStarted`, `running`, `succeeded`, `failed`e `unkownFutureValue``skipped` . |
| tenantId        | String                     | Indica a ID do locatário do enviador. Não é necessário quando criado usando uma `POST` operação. Ele é extraído do token da chamada pós-API. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.threatSubmission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.threatSubmission",
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
  "clientSource": "String"
}
```

