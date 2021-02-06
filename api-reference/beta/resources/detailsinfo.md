---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter informações sobre a identidade ou o sistema associado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 25441071581af0b9e35ef941d8c82998bdea7b38
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135650"
---
# <a name="detailsinfo-resource-type"></a>Tipo de recurso detailsInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um pacote de propriedades que pode conter informações sobre a identidade ou o sistema associado. Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.

## <a name="properties"></a>Propriedades
O **recurso detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais, como **ApplicationId**, **ObjectId** e **UPN**. O conjunto de propriedades varia com base no tipo de recurso que está sendo provisionado. [Listar provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.

## <a name="relationships"></a>Relações
Nenhuma
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


