---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 675c3dd641f435a54775bc7a5b1e5755f270a8d61a6aa03c695496f43ef8406e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .DeleteAsync();

```