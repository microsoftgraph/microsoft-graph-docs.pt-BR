---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab6c33e99f188d67ee6f11f4bbc54191c6a95972
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365GroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```