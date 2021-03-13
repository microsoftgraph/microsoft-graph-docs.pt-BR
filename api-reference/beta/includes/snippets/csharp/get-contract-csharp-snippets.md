---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7b14f7e60917d8fe11406770fc09b5b8be51cf6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contract = await graphClient.Contracts["{contract-id}"]
    .Request()
    .GetAsync();

```