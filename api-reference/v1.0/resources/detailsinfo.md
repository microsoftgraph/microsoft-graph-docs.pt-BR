---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240761"
---
# <a name="detailsinfo-resource-type"></a>Tipo de recurso detailsInfo

Namespace: microsoft.graph

Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado. Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.

## <a name="properties"></a>Propriedades
O **recurso detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais, como **ApplicationId,** **ObjectId** e **UPN**. O conjunto de propriedades varia de acordo com o tipo de recurso que está sendo provisionado. [A lista provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.

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


