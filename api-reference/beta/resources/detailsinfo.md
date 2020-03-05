---
title: tipo de recurso detailsInfo
description: Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 434cc659c66c94b3120431c233fe583e87bfbbbd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507258"
---
# <a name="detailsinfo-resource-type"></a>tipo de recurso detailsInfo

Namespace: Microsoft. Graph

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
