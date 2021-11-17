---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: add55f90457159609fecb26e531b0e782f36a738cdca5fbbf04955fb5d2d5488
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899487"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Websites["{personWebsite-id}"]
    .Request()
    .DeleteAsync();

```