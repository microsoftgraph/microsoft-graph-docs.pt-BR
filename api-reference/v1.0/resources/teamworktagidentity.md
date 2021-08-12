---
title: Tipo de recurso teamworkTagIdentity
description: Representa uma marca em Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2f507844751b92493eab2c4bb84f2da2f3a04c8afb310b682ac9beb2f025031f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129936"
---
# <a name="teamworktagidentity-resource-type"></a>Tipo de recurso teamworkTagIdentity

Namespace: microsoft.graph

Representa uma **marca** em Microsoft Teams. As marcas permitem que os usuários se conectem rapidamente ao subconjunto de usuários em uma equipe. Para obter detalhes sobre o gerenciamento de marca Microsoft Teams, consulte [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). Nome de exibição da marca.|
|id|Cadeia de caracteres|Herdado da [identidade](../resources/identity.md). ID da marca.|

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

