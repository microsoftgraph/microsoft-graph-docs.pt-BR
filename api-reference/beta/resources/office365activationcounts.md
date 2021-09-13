---
title: Tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 33a39a394b5b82bfb3ba0b5d33dc91320307bb73
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115146"
---
# <a name="office365activationcounts-resource-type"></a>Tipo de recurso office365ActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| productType       | Cadeia de Caracteres | O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client". |
| windows           | Int64  | A contagem de ativação Windows. Esse número inclui todas as ativações em qualquer computador Windows computador. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| ios               | Int64  | A contagem de ativação no iOS.             |
| windows10Mobile   | Int64  | A contagem de ativação Windows 10 celular. |

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


