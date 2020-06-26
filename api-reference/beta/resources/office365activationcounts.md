---
title: tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 1e514eb538b1edc4d9681b9937fe8cfeecc40b23
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896886"
---
# <a name="office365activationcounts-resource-type"></a>tipo de recurso office365ActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A última data do conteúdo.          |
| ProductType       | String | O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client". |
| Windows           | Int64  | A contagem de ativação no Windows. Esse número inclui todas as ativações em qualquer computador Windows. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| Android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| emiti               | Int64  | A contagem de ativação no iOS.             |
| windows10Mobile   | Int64  | A contagem de ativação no Windows 10 Mobile. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "windows": 1024, 
  "mac": 1024, 
  "android": 1024, 
  "ios": 1024, 
  "windows10Mobile": 1024
}
```
