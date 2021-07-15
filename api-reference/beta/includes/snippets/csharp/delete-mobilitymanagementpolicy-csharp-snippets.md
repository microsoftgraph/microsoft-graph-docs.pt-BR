---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a046bc7711013c95724ee67e19031febc63d6de4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.MobileDeviceManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .DeleteAsync();

```