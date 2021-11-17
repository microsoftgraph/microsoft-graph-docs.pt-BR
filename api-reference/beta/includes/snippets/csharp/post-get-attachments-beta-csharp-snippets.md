---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93557b1c04afb6313b59a1ff6f779f6b0ccf062d797dd124a68890e5c3682321
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachments = await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Attachments
    .Request()
    .GetAsync();

```