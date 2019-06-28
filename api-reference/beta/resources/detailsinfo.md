---
title: tipo de recurso detailsInfo
description: Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349316"
---
# <a name="detailsinfo-resource-type"></a>tipo de recurso detailsInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado. Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.

## <a name="properties"></a>Propriedades
O recurso **detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais como **ApplicationId**, **ObjectID**e **UPN**. O conjunto de propriedades varia com base no tipo de recurso que está sendo provisionado. [List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
