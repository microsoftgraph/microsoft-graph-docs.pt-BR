---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e997c3cfe90057a43be0ff820cd153dbb739a9a7
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetOneDriveActivityUserDetail('D7')
    .Request()
    .GetAsync();

```