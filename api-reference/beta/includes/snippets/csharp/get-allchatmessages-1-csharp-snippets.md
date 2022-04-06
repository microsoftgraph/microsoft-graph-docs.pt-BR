---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f69fd2384088d3ac1103829346fb0864a2552848
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .OrderBy("createdDateTime desc")
    .Top(2)
    .GetAsync();

```