---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b4d4c20cedb526e24a1f0b05d722c8b8d1f7050
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613292"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var masterCategories = await graphClient.Me.Outlook.MasterCategories
    .Request()
    .GetAsync();

```