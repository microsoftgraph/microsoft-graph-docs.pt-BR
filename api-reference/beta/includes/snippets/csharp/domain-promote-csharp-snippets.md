---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd687c990d096492c2c13bcc5bb89cdd0916f2c4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "66446572"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Domains["{domain-id}"]
    .Promote()
    .Request()
    .PostAsync();

```