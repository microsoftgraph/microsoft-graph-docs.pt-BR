---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9c1dbbaa6a429a90a54f8af5f3b380ff58c86dab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007491"
---
# <a name="useractivationcounts-resource-type"></a>tipo de recurso userActivationCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| ProductType       | String | O tipo de produto, como "Office 365 ProPlus", "Project Client" ou "Visio Pro for Office 365". |
| lastActivatedDate | Data   | A data da ativação mais recente.       |
| Windows           | Int64  | A contagem de ativação no Windows. Esse número inclui todas as ativações em qualquer computador Windows. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| windows10Mobile   | Int64  | A contagem de ativação no Windows 10 Mobile. |
| emiti               | Int64  | A contagem de ativação no iOS.             |
| Android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| activatedOnSharedComputer   | Booliano | True se o usuário usou o produto em um computador compartilhado antes. |

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
