---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 325084b0b52e43160fba3eadfcedf73ae6917fb6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```