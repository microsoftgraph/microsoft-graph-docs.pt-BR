---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19449c128fa737b9dd6fc7bec80c000c16b7a226500cc328b9b8cc7841bf46c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213743"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.Print.Shares["{printerShare-id}"].Jobs
    .Request()
    .GetAsync();

```