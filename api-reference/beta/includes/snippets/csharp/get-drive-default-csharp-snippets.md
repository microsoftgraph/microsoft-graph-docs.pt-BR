---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 916b2b7f4abe57399fdc4175347678ba359f215f7be1f3b3ff62cd437694fe2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drive = await graphClient.Me.Drive
    .Request()
    .GetAsync();

```