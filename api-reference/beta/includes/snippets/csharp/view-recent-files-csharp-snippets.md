---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54c7f278b76078fd91bc9627b4f62fa544b75013
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var recent = await graphClient.Me.Drive
    .Recent()
    .Request()
    .GetAsync();

```