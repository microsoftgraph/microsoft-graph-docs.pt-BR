---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be5a5c523727e3ad0b162f4aba5f1c2647ee8486
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "35711477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .GetAsync();

```