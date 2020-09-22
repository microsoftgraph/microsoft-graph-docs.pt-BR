---
title: tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fb971295919f779c3faddb34ceeb96d531011b1f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052569"
---
# <a name="onlinemeetinginfo-resource-type"></a>tipo de recurso onlineMeetingInfo

Namespace: microsoft.graph

Detalhes para o participante entrar na reunião online.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|ID|Cadeia de caracteres| A ID da conferência.|
|joinUrl|Cadeia de caracteres| O link externo que inicia a reunião online. Esta é uma URL que os clientes serão inicializados em um navegador e redirecionará o usuário para participar da reunião.|
|telefones|Coleção [phone](phone.md)| Todos os números de telefone associados a esta conferência.|
|quickDial|Cadeia de caracteres| O Quickdial pré-formatado para esta chamada.|
|tollFreeNumbers|Coleção de cadeias de caracteres| Os números de chamada gratuita que podem ser usados para ingressar na conferência.|
|tollNumber|Cadeia de caracteres| O número de chamada tarifada que pode ser usado para ingressar na conferência.|

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


