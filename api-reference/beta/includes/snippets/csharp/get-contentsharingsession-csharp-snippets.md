---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 105227819f82fe5afcf5770b0fdb5c3da7f9211f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210303"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contentSharingSession = await graphClient.Communications.Calls["{call-id}"].ContentSharingSessions["{contentSharingSession-id}"]
    .Request()
    .GetAsync();

```