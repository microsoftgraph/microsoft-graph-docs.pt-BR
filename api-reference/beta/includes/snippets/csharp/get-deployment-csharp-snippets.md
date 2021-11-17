---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94c02aca2dcba8c3931c4fc6830741749fc4929d41009633120901202f19379d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployment = await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"]
    .Request()
    .GetAsync();

```