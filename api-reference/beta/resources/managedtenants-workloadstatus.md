---
title: Tipo de recurso workloadStatus
description: Represente o status de uma carga de trabalho.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 50cbd9cdc59426f413333835c4418112401d8038
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402125"
---
# <a name="workloadstatus-resource-type"></a>Tipo de recurso workloadStatus

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represente o status de uma carga de trabalho.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da carga de trabalho. Obrigatório. Somente leitura.|
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
