---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c67f95907863d43d9080bcc59ca0765fe7aac3595b0e28b45d4fd2d7f9b8d30f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = await graphClient.Me.Profile.Addresses["{itemAddress-id}"]
    .Request()
    .GetAsync();

```