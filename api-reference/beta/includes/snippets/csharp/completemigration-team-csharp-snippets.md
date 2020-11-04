---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41c43d7b86c49ce07a63011493a79811c712178c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"]
    .CompleteMigration()
    .Request()
    .PostAsync();

```