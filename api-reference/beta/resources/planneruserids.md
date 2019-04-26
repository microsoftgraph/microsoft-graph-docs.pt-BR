---
title: tipo de recurso plannerUserIds
description: O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um plano é compartilhado. Este é um tipo aberto. Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano do grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 83717714d58cd0c442b42c23c9aa361bcd3b2261
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344363"
---
# <a name="planneruserids-resource-type"></a>tipo de recurso plannerUserIds

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerUserIds** representa a lista de IDs de usuários com as quais um [plano](plannerplan.md) é compartilhado. Este é um tipo aberto. Se estiver aproveitando os grupos do Office 365, use a API de grupos para gerenciar a associação de grupo para compartilhar o plano [do grupo](group.md) . Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de Propriedade do grupo.


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer IDs de usuário como propriedades com seus valores como `true` Boolean. Quando as IDs de usuário não são mais compartilhadas, as propriedades são removidas automaticamente `false` definindo seus valores para o Boolean.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
