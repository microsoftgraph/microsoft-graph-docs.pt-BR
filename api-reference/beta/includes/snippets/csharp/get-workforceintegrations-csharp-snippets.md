---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b490bb63616cd5aa1f98b586b4e01c1da5f452afe6ba155d23b3a32bc400f188
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159558"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workforceIntegrations = await graphClient.Teamwork.WorkforceIntegrations
    .Request()
    .GetAsync();

```