---
title: Tipo de recurso privilegedRoleSettings
description: Representa as configurações de uma função privilegiada.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: b954dbc0dc72028d60861c5c07820302f3cbe19d
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454119"
---
# <a name="privilegedrolesettings-resource-type"></a>Tipo de recurso privilegedRoleSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de uma função privilegiada.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Ler propriedades e relações do objeto privilegedRoleSettings.|
|[Atualizar privilegedRoleSettings](../api/privilegedrolesettings-update.md) | [privilegedRoleSettings](privilegedrolesettings.md) |Atualize o objeto privilegedRoleSettings.|
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|elevationDuration|duração|A duração quando a função é ativada.|
|id|string| O identificador exclusivo para as configurações de função. Somente leitura.|
|isMfaOnElevationConfigurable|booliano|`true` se **mfaOnElevation** for configurável. `false` se **mfaOnElevation** não for configurável.|
|lastGlobalAdmin|booliano|Somente uso interno.|
|maxElavationDuration|duração|Duração máxima da função ativada.|
|mfaOnElevation|booliano|`true` se o MFA for necessário para ativar a função. `false` se o MFA não for necessário para ativar a função.|
|minElevationDuration|duração|Duração mínima para a função ativada.|
|notificationToUserOnElevation|booliano|`true` se enviar notificação ao usuário final quando a função for ativada. `false` se não enviar notificação quando a função for ativada.|
|ticketingInfoOnElevation|booliano|`true` se as informações de tíquete são necessárias ao ativar a função. `false` se as informações de tíquete não são necessárias ao ativar a função.|
|approvalOnElevation|booliano|`true` se a aprovação for necessária ao ativar a função. `false` se a aprovação não for necessária ao ativar a função.|
|approverIds| coleção de cadeias de caracteres |Lista de IDs de Aprovação, se a aprovação for necessária para ativação.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSettings"
}-->

```json
{
  "elevationDuration": "String (timestamp)",
  "id": "string (identifier)",
  "isMfaOnElevationConfigurable": true,
  "lastGlobalAdmin": true,
  "maxElavationDuration": "String (timestamp)",
  "mfaOnElevation": true,
  "minElevationDuration": "String (timestamp)",
  "notificationToUserOnElevation": true,
  "ticketingInfoOnElevation": true,
  "approvalOnElevation": false,
  "approverIds": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


