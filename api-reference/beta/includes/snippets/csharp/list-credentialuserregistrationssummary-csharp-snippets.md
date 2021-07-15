---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8594a1db0159d600f47fd53df2768bfdabe01738
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var credentialUserRegistrationsSummaries = await graphClient.TenantRelationships.ManagedTenants.CredentialUserRegistrationsSummaries
    .Request()
    .GetAsync();

```