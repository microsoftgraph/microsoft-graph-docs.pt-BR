---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: baa50e86ddd406b31c0f4df1bb34097b9bbc077a06bf160213d016044260c3b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275091"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var participants = new List<String>()
{
    ""
};

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["{call-id}"].Participants
    .MuteAll(participants,clientContext)
    .Request()
    .PostAsync();

```