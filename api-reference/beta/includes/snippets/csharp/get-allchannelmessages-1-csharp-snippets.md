---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf92f72a6dd9ae442fa26c702bba27beec5c131
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getAllMessages = await graphClient.Teams["{team-id}"].Channels
    .GetAllMessages()
    .Request()
    .GetAsync();

```