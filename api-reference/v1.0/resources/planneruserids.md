---
title: Tipo de recurso plannerUserIds
description: O **recurso plannerUserIds** representa a lista de IDs de usuários com as que um plano é compartilhado. Este é um Tipo Aberto. Se você estiver aproveitando Microsoft 365 grupos, use a API grupos para gerenciar a associação ao grupo para compartilhar o plano do grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de propriedade do grupo.
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 53b10f1f1ca921446279c294782ceb68dbf182f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021439"
---
# <a name="planneruserids-resource-type"></a>Tipo de recurso plannerUserIds

Namespace: microsoft.graph

O **recurso plannerUserIds** representa a lista de IDs de usuários com as que um [plano](plannerplan.md) é compartilhado. Este é um Tipo Aberto. Se você estiver aproveitando Microsoft 365 grupos, use a API grupos para gerenciar a associação ao grupo para compartilhar o [plano do](group.md) grupo. Você também pode adicionar membros existentes do grupo a essa coleção, embora não seja necessário que eles acessem o plano de propriedade do grupo.


## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer ids de usuário como propriedades, com seus valores sendo `true` booleano. Quando as ids do usuário não são mais compartilhadas, as propriedades são removidas automaticamente definindo seus valores como `false` booleano.


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

### <a name="example"></a>Exemplo
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

