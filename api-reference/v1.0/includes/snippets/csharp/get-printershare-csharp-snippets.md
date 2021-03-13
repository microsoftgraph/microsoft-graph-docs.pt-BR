---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 747588e72f9a085fca3ff3f05a1165dffb513de1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771600"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .GetAsync();

```