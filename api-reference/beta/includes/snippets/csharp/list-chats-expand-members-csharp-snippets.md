---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdc112067fdf30fd5f13df1f4dd46b89a29294fb9adc4b4b9248ee5a88de1e09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chats = await graphClient.Users["{user-id}"].Chats
    .Request()
    .Expand("members")
    .GetAsync();

```