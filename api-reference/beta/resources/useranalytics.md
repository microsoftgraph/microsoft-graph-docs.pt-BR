---
title: tipo de recurso useranalytics
description: As configurações do usuário e as estatísticas de atividade.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ffe6830088bd60c4de9cea8def8e8202d1b33f13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519537"
---
# <a name="useranalytics-resource-type"></a>tipo de recurso useranalytics

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações do usuário e as estatísticas de atividade.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
[Obter configurações](../api/useranalytics-get-settings.md) | [configurações](settings.md) | Obter as configurações do usuário para usar a API de análise.|

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|configurações|[configurações](settings.md)|As configurações atuais de um usuário para usar a API de análise.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|activityStatistics|coleção [activityStatistics](activitystatistics.md)| O conjunto de atividades de trabalho que um usuário gastou enquanto está fora do horário de trabalho. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "activityStatistics"
  ],
  "@odata.type": "microsoft.graph.userAnalytics"
}-->

```json
{
  "id": "string",
  "settings": {"@odata.type": "microsoft.graph.settings"},
  "activityStatistics": [{"@odata.type": "microsoft.graph.activityStatistics"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userAnalytics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
