---
title: Tipo de recurso office365ActivationCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 39e679da134120377f17dab520c332dc54aab328ef924b65212f5145279a8402
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176320"
---
# <a name="office365activationcounts-resource-type"></a>Tipo de recurso office365ActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| reportRefreshDate | Data   | A data mais recente do conteúdo.          |
| productType       | Cadeia de caracteres | O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client". |
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


