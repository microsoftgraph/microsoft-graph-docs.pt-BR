---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91366f9d2b2308c997c111123d856581db7c00c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43384951"
---
# <a name="useractivationcounts-resource-type"></a>tipo de recurso userActivationCounts

Namespace: microsoft.graph

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
