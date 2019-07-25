---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0888f99c2da0186dcd89c38a022ff7463665c22
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityFileCounts('D7')
    .Request()
    .GetAsync();

```