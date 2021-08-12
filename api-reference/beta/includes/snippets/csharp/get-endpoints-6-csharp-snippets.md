---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9766b56a7151e81316886ad3b832a5825d55cfb7be308321de65da667be26688
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByUser = await graphClient.Print.Reports.MonthlyPrintUsageByUser
    .Request()
    .GetAsync();

```