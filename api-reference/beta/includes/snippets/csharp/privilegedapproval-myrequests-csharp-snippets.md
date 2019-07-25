---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29fc83fa1a808fbaa980ed8857abdb10ef5fc857
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875899"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var myRequests = await graphClient.PrivilegedApproval
    .MyRequests()
    .Request()
    .GetAsync();

```