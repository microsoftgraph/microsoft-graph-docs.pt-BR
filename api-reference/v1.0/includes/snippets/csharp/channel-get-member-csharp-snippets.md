---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf65874911b8ccc30432543342c0f891fb9a7241d630b57197b7ea2fac641106
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159518"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```