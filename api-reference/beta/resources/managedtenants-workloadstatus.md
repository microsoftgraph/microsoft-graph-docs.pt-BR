---
title: Tipo de recurso workloadStatus
description: Represente o status de uma carga de trabalho.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d85d7fd60a269c360185d8d4ffb5952a71bdd628
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792264"
---
# <a name="workloadstatus-resource-type"></a>Tipo de recurso workloadStatus

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represente o status de uma carga de trabalho.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da carga de trabalho. Obrigatório. Somente leitura.|
|offboardedDateTime|DateTimeOffset|A data e a hora em que a carga de trabalho foi desligada. Opcional. Somente leitura.|
|onboardedDateTime|DateTimeOffset|A data e a hora em que a carga de trabalho foi internada. Opcional. Somente leitura.|
|onboardingStatus|workloadOnboardingStatus|O status de integração da carga de trabalho. Os valores possíveis são: `notOnboarded`, `onboarded`, `unknownFutureValue`. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.workloadStatus",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "displayName": "String",
  "offboardedDateTime": "String (timestamp)"
}
```
