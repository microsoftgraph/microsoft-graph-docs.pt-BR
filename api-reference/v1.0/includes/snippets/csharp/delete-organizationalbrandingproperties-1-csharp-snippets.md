---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2daa0fe4cbf0c55250db3d46592a1cb174428e1dadee295eff9f72b472961de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organization-id}"].Branding
    .Request()
    .DeleteAsync();

```