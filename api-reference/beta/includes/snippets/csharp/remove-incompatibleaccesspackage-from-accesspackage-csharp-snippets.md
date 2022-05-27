---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d358a75d0da31c30fc60d531fad0527c63ae94b5dbd471e4db10daf1f2377383
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages["{accessPackage-id}"].Reference
    .Request()
    .DeleteAsync();

```