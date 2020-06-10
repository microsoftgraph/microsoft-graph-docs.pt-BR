---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81fe099c7b3f7ade3696158e3bbf1e8beb05d9fe
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkAGVmMDEz"]
    .Request()
    .Select("internetMessageHeaders")
    .GetAsync();

```