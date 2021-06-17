---
title: Tipo de recurso cloudPcUserSettingAssignment
description: Representa uma coleção definida de atribuições de configuração do usuário.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 704142ce266a826606b6c32b209d69d052d1a3c9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993654"
---
# <a name="cloudpcusersettingassignment--resource-type"></a>Tipo de recurso cloudPcUserSettingAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma coleção definida de atribuições de configuração do usuário.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da atribuição de configuração do usuário. Somente leitura. Se `target` for um grupo de usuários, a ID terá essa estrutura: {policyID}_{groupID}.|
|destino|[cloudPcManagementAssignmentTarget](../resources/cloudpcmanagementassignmenttarget.md)|O destino de atribuição para a configuração do usuário. Atualmente, o único destino com suporte para a configuração do usuário é um grupo de usuários.|
|createdDateTime|DateTimeOffset|A data e a hora em que essa atribuição foi criada. O tipo Timestamp representa as informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 tem esta aparência: '2014-01-01T00:00:00Z'.  |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
