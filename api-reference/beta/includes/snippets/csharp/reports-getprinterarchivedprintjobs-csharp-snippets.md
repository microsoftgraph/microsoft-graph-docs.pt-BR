---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 943ede8fc0dcf9ee4cf91ecdef8f8ea86c4f31408df8f85619fa94ef52a8abc2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getPrinterArchivedPrintJobs = await graphClient.Print.Reports
    .GetPrinterArchivedPrintJobs("016b5565-3bbf-4067-b9ff-4d68167eb1a6","2021-05-24","2021-05-25")
    .Request()
    .GetAsync();

```