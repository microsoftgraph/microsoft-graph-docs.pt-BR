---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5267e28db93e3fdc68159170c2647c5a36f841dc
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactMergeSuggestions = await graphClient.Me.Settings.ContactMergeSuggestions
    .Request()
    .GetAsync();

```