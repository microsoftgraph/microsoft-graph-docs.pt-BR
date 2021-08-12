---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a7748973f251c0dfa3e5efa669167c49847b05bc5d4afb145de78fb30949ab6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237015"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Users["AlexW@contoso.OnMicrosoft.com"].Calendar
    .Request()
    .GetAsync();

```