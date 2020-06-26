---
title: tipo de recurso plannerUserIds
description: O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um plano é compartilhado. Este é um tipo aberto. Se você estiver aproveitando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano do grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 3cd4007c4ae68cfe9428eb6b9d2aeb22cd24391e
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896984"
---
# <a name="planneruserids-resource-type"></a>tipo de recurso plannerUserIds

Namespace: microsoft.graph

O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um [plano](plannerplan.md) é compartilhado. Este é um tipo aberto. Se você estiver aproveitando os grupos do Microsoft 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) . Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer IDs de usuário como propriedades com seus valores como `true` Boolean. Quando as IDs de usuário não são mais compartilhadas, as propriedades são removidas automaticamente definindo seus valores para o `false` Boolean.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

Como
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
