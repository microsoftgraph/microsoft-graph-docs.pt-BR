---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7874884676f6f770daf66be533f6933260907edc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUserHistoryItem = await graphClient.RiskyUsers["{riskyUser-id}"].History["{riskyUserHistoryItem-id}"]
    .Request()
    .GetAsync();

```