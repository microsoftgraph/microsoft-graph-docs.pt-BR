---
title: tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6433c1680630b5805cd18a22e550e58a51bcefbc
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898300"
---
# <a name="useractivationcounts-resource-type"></a>tipo de recurso userActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| ProductType       | String | O tipo de produto, como "Microsoft 365 ProPlus" ou "Project Client". |
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
