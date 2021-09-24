---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec4896bb1c34aebace04636d7bcd782d1cf6de8b8073466d554aa5b7bfe6bb43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .DeleteAsync();

```