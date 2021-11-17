---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92a1cc631ca4521808e042225daa2aa74604178a6d8c2da3d60874aabd44f7cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158200"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"]
    .Request()
    .DeleteAsync();

```