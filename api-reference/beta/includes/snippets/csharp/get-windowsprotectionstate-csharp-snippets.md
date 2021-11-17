---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b586c052938a7229eb5d21eb055fbe1d2eaf13462ab7db026c125c9e24db9dc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsProtectionState = await graphClient.TenantRelationships.ManagedTenants.WindowsProtectionStates["{managedTenants.windowsProtectionState-id}"]
    .Request()
    .GetAsync();

```