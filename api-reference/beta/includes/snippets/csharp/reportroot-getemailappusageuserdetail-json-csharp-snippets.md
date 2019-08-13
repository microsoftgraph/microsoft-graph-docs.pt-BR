---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90a36027a959135380dafd58289b74326a9ea3df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308485"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageUserDetail = await graphClient.Reports
    .GetEmailAppUsageUserDetail("D7")
    .Request()
    .GetAsync();

```