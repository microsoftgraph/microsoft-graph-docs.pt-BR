---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 791e84e6bbc9f730bf4e2db756bb1e3e0f839a51
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessPeerToPeerActivityMinuteCounts = await graphClient.Reports
    .GetSkypeForBusinessPeerToPeerActivityMinuteCounts('D7')
    .Request()
    .GetAsync();

```