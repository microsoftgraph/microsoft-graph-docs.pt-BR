---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 021f82ba6f1930b6961764845aab73fd415d2b75
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Groups["{group-id}"].Settings
    .Request()
    .GetAsync();

```