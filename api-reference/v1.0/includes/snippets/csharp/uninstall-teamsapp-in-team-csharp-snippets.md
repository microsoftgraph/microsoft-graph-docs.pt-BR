---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 874a01488f969f34ee2491236a1835b704ea20bb
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690639"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["6903fa93-605b-43ef-920e-77c4729f8258"].InstalledApps["NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="]
    .Request()
    .DeleteAsync();

```