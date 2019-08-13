---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 071750b4f9d0e820861c6edc11db21165bf0a105
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetSkypeForBusinessDeviceUsageUserDetail("D7")
    .Request()
    .GetAsync();

```