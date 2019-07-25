---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcbc062cb8cdbee6409ec23c3503e4b147532624
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887972"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sections = await graphClient.Me.Onenote.Sections
    .Request()
    .GetAsync();

```