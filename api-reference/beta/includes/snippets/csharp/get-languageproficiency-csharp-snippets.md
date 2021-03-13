---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 855bb30a2893745327421732d2a2a77842308b5b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = await graphClient.Me.Profile.Languages["{languageProficiency-id}"]
    .Request()
    .GetAsync();

```