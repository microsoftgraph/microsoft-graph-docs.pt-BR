---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2d97d4f220a4579b805959c3b5d9c369293b2730
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453636"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|Cadeia de caracteres|Metadados de número de tíquete|
|ticketSystem|Cadeia de caracteres|Dados de meta do sistema de tíquetes|

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

