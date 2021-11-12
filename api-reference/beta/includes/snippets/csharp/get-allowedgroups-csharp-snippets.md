---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f68f92a9b9635246ddbb5053587c5244b47f8957326e337215bcbf0ac70732a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899742"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedGroups = await graphClient.Print.Shares["{printerShare-id}"].AllowedGroups
    .Request()
    .GetAsync();

```