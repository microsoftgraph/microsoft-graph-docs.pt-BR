---
title: Tipo de recurso retentionDurationInDays
description: Representa o número de dias que um item será retido antes de ser excluído
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 4f8546d98e5430651ae672737e3d32a5e4744738
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447502"
---
# <a name="retentiondurationindays-resource-type"></a>Tipo de recurso retentionDurationInDays

Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de dias que um item será retido antes de poder ser excluído.


Herda de [retentionDuration](../resources/security-retentionduration.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Dias|Int32|Especifica o período em dias para o qual um item com o rótulo de retenção aplicado será retido.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionDurationInDays"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionDurationInDays",
  "days": "Integer"
}
```