---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb7b25f61430689364202a8d2c42bc0cd1fbb326463f20d52a53019655ec7e2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329991"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .Request()
    .DeleteAsync();

```