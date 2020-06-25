---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1d6850d4a874cda324247fd66bce6f4346edda0
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864146"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{id}"].ClaimsMappingPolicies["{id}"].Reference
    .Request()
    .DeleteAsync();

```