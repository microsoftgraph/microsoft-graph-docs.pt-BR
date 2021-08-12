---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: e5beb5d281186b16acfa38087b6ee2d9ed3f0058f972aaeba2941467c545f523
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130377"
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


