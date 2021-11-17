---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67cef0140628a128a2fecb359c06ec07aed8f6d450e2e8fa979bad9621795a05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159233"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.Chats["{chat-id}"].Operations
    .Request()
    .GetAsync();

```