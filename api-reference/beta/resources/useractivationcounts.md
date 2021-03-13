---
title: Tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 48adb73bac65ddced88aea3edb18deae7653f5b3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761790"
---
# <a name="useractivationcounts-resource-type"></a>Tipo de recurso userActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Cadeia de Caracteres | O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client". |
| lastActivatedDate | Data   | A data da ativação mais recente.       |
| windows           | Int64  | A contagem de ativação no Windows. Esse número inclui todas as ativações em qualquer computador Windows. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| windows10Mobile   | Int64  | A contagem de ativação no Windows 10 mobile. |
| ios               | Int64  | A contagem de ativação no iOS.             |
| android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| activatedOnSharedComputer   | Boolean | True se o usuário usou o produto em um computador compartilhado antes. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userActivationCounts"
} -->

```json
{
  "productType": "String", 
  "lastActivatedDate": "Date", 
  "windows": 1024, 
  "mac": 1024, 
  "windows10Mobile": 1024, 
  "ios": 1024, 
  "android": 1024,
  "activatedOnSharedComputer": true 
}
```


