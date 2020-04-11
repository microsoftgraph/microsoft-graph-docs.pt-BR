---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 063f2f43f98d9f2d75822f712c4e17755bc290f7
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229448"
---
# <a name="onlinemeetinginfo-resource-type"></a>tipo de recurso onlineMeetingInfo

Detalhes para o participante entrar na reunião online.

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
}-->
