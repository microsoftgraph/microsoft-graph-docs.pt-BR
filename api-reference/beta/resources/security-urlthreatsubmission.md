---
title: Tipo de recurso urlThreatSubmission
description: Representar um envio de ameaças relacionado a uma URL
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5f04e14d1482a935868f4a0a7985b43b6faf5188
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856516"
---
# <a name="urlthreatsubmission-resource-type"></a>Tipo de recurso urlThreatSubmission

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representar um envio de ameaças relacionado a uma URL.

Esse recurso é usado para enviar URLs de phishing suspeitas para Microsoft Defender para Office 365. Ele também pode ser usado para enviar casos falsos positivos que não devem ter sido bloqueados, como URLs seguras.

Herda de [threatSubmission](../resources/security-threatsubmission.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar urlThreatSubmissions](../api/security-urlthreatsubmission-list.md)|[coleção microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Obtenha uma lista dos [objetos urlThreatSubmission](../resources/security-urlthreatsubmission.md) e suas propriedades.|
|[Criar urlThreatSubmission](../api/security-urlthreatsubmission-post-urlthreats.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Crie um novo [objeto urlThreatSubmission](../resources/security-urlthreatsubmission.md) .|
|[Obter urlThreatSubmission](../api/security-urlthreatsubmission-get.md)|[microsoft.graph.security.urlThreatSubmission](../resources/security-urlthreatsubmission.md)|Leia as propriedades e as relações de um [objeto urlThreatSubmission](../resources/security-urlthreatsubmission.md) .|

## <a name="properties"></a>Propriedades
| Propriedade | Tipo   | Descrição                 |
|:---------|:-------|:----------------------------|
| webUrl   | String | Indica a webUrl que precisa ser enviada. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.urlThreatSubmission",
  "baseType": "microsoft.graph.security.threatSubmission",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.urlThreatSubmission",
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
  "webUrl": "String"
}
```

