---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 571b02af24fdc5c425148f826259a79456db355ddbe27880c3050ac8c91a63b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAllMessages = await graphClient.Teams["{team-id}"].Channels
    .GetAllMessages()
    .Request()
    .GetAsync();

```