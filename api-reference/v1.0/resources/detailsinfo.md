---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: f755e7014e1a381697874e3e8da1afe72fa51fe0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104212"
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


