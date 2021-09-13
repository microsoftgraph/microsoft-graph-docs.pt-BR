---
title: Tipo de recurso onlineMeetingInfo
description: Detalhes para o participante entrar na reunião online.
ms.localizationpriority: medium
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 325840e11b93658abe3294edf339175bebe03daf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023224"
---
# <a name="onlinemeetinginfo-resource-type"></a>Tipo de recurso onlineMeetingInfo

Namespace: microsoft.graph

Detalhes para o participante entrar na reunião online.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|conferenceId|Cadeia de caracteres| A ID da conferência.|
|joinUrl|String| O link externo que inicia a reunião online. Essa é uma URL que os clientes iniciarão em um navegador e redirecionam o usuário para ingressar na reunião.|
|telefones|Coleção [phone](phone.md)| Todos os números de telefone associados a essa conferência.|
|quickDial|Cadeia de caracteres| O quickdial pré-formatado para essa chamada.|
|tollFreeNumbers|String collection| Os números gratuitos que podem ser usados para ingressar na conferência.|
|tollNumber|Cadeia de Caracteres| O número de telefone que pode ser usado para ingressar na conferência.|

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


