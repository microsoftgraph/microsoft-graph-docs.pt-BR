---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b777e6ecccdabfaa6aac5c6a3a4efe04f878e92bab7e82d15adbd436b8cc738
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407132"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsTab = await graphClient.Chats["{chat-id}"].Tabs["{teamsTab-id}"]
    .Request()
    .Expand("teamsApp")
    .GetAsync();

```