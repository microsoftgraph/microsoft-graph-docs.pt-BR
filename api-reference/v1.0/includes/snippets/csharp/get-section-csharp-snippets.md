---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f63b3a4336d4421cc92d1347c58203cf518b9aa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785866"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = await graphClient.Me.Onenote.Sections["{onenoteSection-id}"]
    .Request()
    .GetAsync();

```