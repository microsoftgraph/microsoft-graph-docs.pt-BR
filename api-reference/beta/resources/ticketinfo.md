---
title: Tipo de recurso ticketInfo
description: O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a59b62ddb014dedd802af6fcde001d4791d729c3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682597"
---
# <a name="ticketinfo-resource-type"></a>Tipo de recurso ticketInfo

Namespace: microsoft.graph

O objeto que representa informações de tíquete relacionadas a solicitações de atribuição de função

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ticketNumber|String|Metadados de número de tíquete|
|ticketSystem|String|Dados de meta do sistema de tíquetes|

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

