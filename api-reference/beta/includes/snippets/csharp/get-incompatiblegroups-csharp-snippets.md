---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3c834521caaef77ab8b75b478a4d7020a465796
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439914"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var incompatibleGroups = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleGroups
    .Request()
    .GetAsync();

```