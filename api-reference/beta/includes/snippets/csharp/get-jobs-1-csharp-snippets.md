---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e19e97babb3743a32096e1d53afd550941e65ec528eaae5a691e2851462191e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214090"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Printers["{printer-id}"].Jobs
    .Request()
    .GetAsync();

```