---
title: tipo de recurso onlineMeetingInfo
description: Detalhes de um participante para ingressar na reunião online.
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939387"
---
# <a name="onlinemeetinginfo-resource-type"></a>tipo de recurso onlineMeetingInfo

Detalhes de um participante para ingressar na reunião online.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ID|String| A ID da conferência.|
|joinUrl|String| O link externo que inicia a reunião online. Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.|
|telefones|Coleção [phone](phone.md)| Todos os números de telefone associados a esta conferência.|
|quickDial|String| O Quickdial pré-formatado para esta chamada.|
|tollFreeNumbers|String collection| Os números de chamada gratuita que podem ser usados para ingressar na conferência.|
|tollNumber|String| O número de chamada tarifada que pode ser usado para ingressar na conferência.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s
