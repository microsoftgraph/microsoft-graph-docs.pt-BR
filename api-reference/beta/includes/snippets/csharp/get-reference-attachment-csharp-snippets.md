---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac63ce78af68696151c0ed7f80068cc72a8168946685bf669d1d5e5962309e9f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["{event-id}"].Attachments["{attachment-id}"]
    .Request()
    .GetAsync();

```