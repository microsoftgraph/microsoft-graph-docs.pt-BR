---
title: Tipo de recurso cloudPcSubscription
description: Representa uma assinatura do PC na nuvem.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 425ada12758e2602d8cf262e27c34087722bf84f
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366297"
---
# <a name="cloudpcsubscription-resource-type"></a>Tipo de recurso cloudPcSubscription

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de assinatura que podem ser usadas para armazenar um instantâneo ou instantâneos de um PC na nuvem para análise forense.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|subscriptionId|Cadeia de caracteres|A ID da assinatura.|
|subscriptionName|String|O nome da assinatura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "subscriptionId",
  "@odata.type": "microsoft.graph.cloudPcSubscription",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSubscription",
  "subscriptionId": "String",
  "subscriptionName": "String"
}
```
