---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6f4305e3b3b75533309d453ef6a5d10bef033e936226189debaf89d6ddbc031
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327737"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = RejectReason.None;

await graphClient.Communications.Calls["{call-id}"]
    .Reject(reason,null)
    .Request()
    .PostAsync();

```