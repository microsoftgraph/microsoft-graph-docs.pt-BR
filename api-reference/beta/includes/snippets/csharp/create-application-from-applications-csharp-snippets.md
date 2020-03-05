---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 187b208ac240947df0b17165815873eca3a18f51
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "38000160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
    DisplayName = "Display name"
};

await graphClient.Applications
    .Request()
    .AddAsync(application);

```