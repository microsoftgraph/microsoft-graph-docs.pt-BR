---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1072f3da89344c07883d25b6cef2e8c75d86ae23
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messages = await graphClient.Chats["{chat-id}"].Messages
    .Request()
    .Top(2)
    .GetAsync();

```