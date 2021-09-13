---
title: Tipo de recurso teamworkTagIdentity
description: Representa uma marca em Microsoft Teams.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7cd605a42f0f0c7f697c7b291fe30645bdf4403b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128169"
---
# <a name="teamworktagidentity-resource-type"></a>Tipo de recurso teamworkTagIdentity

Namespace: microsoft.graph

Representa uma **marca** em Microsoft Teams. As marcas permitem que os usuários se conectem rapidamente ao subconjunto de usuários em uma equipe. Para obter detalhes sobre o gerenciamento de marca Microsoft Teams, consulte [Manage tags in Microsoft Teams](/microsoftteams/manage-tags).


Herda da [identidade](../resources/identity.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Herdado da [identidade](../resources/identity.md). Nome de exibição da marca.|
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

