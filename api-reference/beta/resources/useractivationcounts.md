---
title: tipo de recurso de userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: cae194545f13d312ee78b572659017752e43a6a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845287"
---
# <a name="useractivationcounts-resource-type"></a>tipo de recurso de userActivationCounts

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Cadeia de caracteres | O tipo de produto, como "Office 365 ProPlus", "Cliente do projeto," ou "Visio Pro para Office 365". |
| lastActivatedDate | Data   | A data da ativação mais recente.       |
| Windows           | Int64  | A contagem de ativação do Windows. Esse número inclui cada ativação em qualquer computador do Windows. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| windows10Mobile   | Int64  | A ativação contar com 10 do Windows mobile. |
| IOS               | Int64  | A contagem de ativação no iOS.             |
| Android           | Int64  | A contagem de ativação em um dispositivo Android.  |
| activatedOnSharedComputer   | Booliano | True se o usuário utilizou o produto em um computador compartilhado antes. |

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
