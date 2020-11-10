---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0e7c7da165658367276b0302dda5f1d780fe037
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974129"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

OutlookTask outlookTask = graphClient.me().outlook().tasks("AAMkADA1MHgwAAA=")
    .buildRequest( requestOptions )
    .get();

```