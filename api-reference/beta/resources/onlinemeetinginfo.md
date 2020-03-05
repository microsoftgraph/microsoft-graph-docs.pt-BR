---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac6c42f28ed1f2adccd54fcd3bd6667f4113b7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522246"
---
# <a name="onlinemeetinginfo-resource-type"></a>tipo de recurso onlineMeetingInfo

Namespace: Microsoft. Graph

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
}-->s
