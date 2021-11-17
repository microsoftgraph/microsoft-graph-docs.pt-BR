---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6358b9bc1e80c6b7e3597594559cfc8e3e9a94c854453ec7488f119e01f4f94d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100366"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipal-id}"].Synchronization.Jobs["{synchronizationJob-id}"].Schema
    .Request()
    .GetAsync();

```