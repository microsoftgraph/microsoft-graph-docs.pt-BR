---
title: Tipo de recurso userActivationCounts
description: Veja a seguir uma representação JSON do recurso.
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 466ccc3f942bec2fbb09e094e7805c4fcf160e54
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033165"
---
# <a name="useractivationcounts-resource-type"></a>Tipo de recurso userActivationCounts

Namespace: microsoft.graph

## <a name="properties"></a>Propriedades

| Propriedade          | Tipo   | Descrição                              |
| :---------------- | :----- | ---------------------------------------- |
| productType       | Cadeia de caracteres | O tipo de produto, como "Microsoft 365 ProPlus"ou "Project Client". |
| lastActivatedDate | Data   | A data da ativação mais recente.       |
| windows           | Int64  | A contagem de ativação Windows. Esse número inclui todas as ativações em qualquer computador Windows computador. |
| mac               | Int64  | A contagem de ativação no Mac OS.          |
| windows10Mobile   | Int64  | A contagem de ativação Windows 10 celular. |
| ios               | Int64  | A contagem de ativação no iOS.             |
| android           | Int64  | A contagem de ativação em um dispositivo Android.  |
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


