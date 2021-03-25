---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe90fb700f30951a4178cb63b49bcbd4b5cfc8da
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202381"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .GetAsync();

```