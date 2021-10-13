---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8f0aee3ddb5ceddce7909bf4b8bbfb7e096ed996ec3728dbeb88c233f7a2f88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tabs = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Tabs
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```