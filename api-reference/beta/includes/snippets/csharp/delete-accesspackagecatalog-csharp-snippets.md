---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 349f772f0edd3a9b356443272401530fe48afeafb1e4f4b829d6f20903a434fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898765"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{accessPackageCatalog-id}"]
    .Request()
    .DeleteAsync();

```