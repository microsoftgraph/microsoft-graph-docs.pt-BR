---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a573e35a6fd6fec71cffaa7f9521b3829af80bf1e43fcda468c096089bf5596
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Messages["{message-id}"].Attachments["{attachment-id}"]
    .Request()
    .Expand("itemattachment/item")
    .GetAsync();

```