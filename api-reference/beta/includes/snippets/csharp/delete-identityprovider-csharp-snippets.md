---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2510def09068f4edb0cf9977874474c3af11b1a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .DeleteAsync();

```