---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d64bd63615ec156548942d14deb5833eb5dd990a
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399450"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|Cadeia de caracteres|Metadados de número de tíquete|
|ticketSystem|Cadeia de caracteres|Metadados do sistema de tíquetes|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ticketInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ticketInfo",
  "ticketNumber": "String",
  "ticketSystem": "String"
}
```

