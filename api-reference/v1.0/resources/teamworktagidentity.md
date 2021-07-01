---
title: Tipo de recurso teamworkTagIdentity
description: Representa uma marca em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b9ea11746a98fba8bb209112c1cb6b1ed63fc954
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211064"
---
# <a name="teamworktagidentity-resource-type"></a>Tipo de recurso teamworkTagIdentity

Namespace: microsoft.graph

Representa uma **marca** em Microsoft Teams. As marcas permitem que os usuários se conectem rapidamente ao subconjunto de usuários em uma equipe. Para obter detalhes sobre o gerenciamento de marca Microsoft Teams, consulte [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição da marca.|
|id|String|Herdado da [identidade](../resources/identity.md). ID da marca.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkTagIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkTagIdentity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

