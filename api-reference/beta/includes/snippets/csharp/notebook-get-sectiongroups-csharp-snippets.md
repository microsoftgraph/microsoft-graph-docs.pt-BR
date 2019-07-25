---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 420e4f209a5ffe7a196ca697b73d6f1b4d6674f0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879035"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sectionGroups = await graphClient.Me.Onenote.Notebooks["{id}"].SectionGroups
    .Request()
    .GetAsync();

```