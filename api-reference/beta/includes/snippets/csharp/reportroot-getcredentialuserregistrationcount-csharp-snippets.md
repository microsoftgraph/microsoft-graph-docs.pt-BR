---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc8e2ba1d5b874acf69e6d63cb3ea06109170a9f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCredentialUserRegistrationCount = await graphClient.Reports
    .GetCredentialUserRegistrationCount()
    .Request()
    .GetAsync();

```