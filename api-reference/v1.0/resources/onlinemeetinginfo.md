---
title: Tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f2a114ed51217e88cf981208b3b010f82a1524221724c8edf2479efc5758ec25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202165"
---
# <a name="onlinemeetinginfo-resource-type"></a>Tipo de recurso onlineMeetingInfo

Detalhes para o participante entrar na reunião online.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|conferenceId|String| A ID da conferência.|
|joinUrl|Cadeia de caracteres| O link externo que inicia a reunião online. Essa é uma URL que os clientes iniciarão em um navegador e redirecionam o usuário para ingressar na reunião.|
|telefones|Coleção [phone](phone.md)| Todos os números de telefone associados a essa conferência.|
|quickDial|Cadeia de caracteres| O quickdial pré-formatado para essa chamada.|
|tollFreeNumbers|Coleção de cadeias de caracteres| Os números gratuitos que podem ser usados para ingressar na conferência.|
|tollNumber|String| O número de telefone que pode ser usado para ingressar na conferência.|

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

