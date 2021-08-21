---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7dd8c6081317180e870344f3b6b9a4675353806632adbf7391ccc4cc18bfc093
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100796"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myRequests = await graphClient.PrivilegedApproval
    .MyRequests()
    .Request()
    .GetAsync();

```