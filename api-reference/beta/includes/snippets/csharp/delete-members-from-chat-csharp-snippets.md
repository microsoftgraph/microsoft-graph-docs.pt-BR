---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95a44311b0de115ca247515164729b44f96dc8e5cbe4b9e56ffcaa6942236e12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Chats["{chat-id}"].Members["{conversationMember-id}"]
    .Request()
    .DeleteAsync();

```