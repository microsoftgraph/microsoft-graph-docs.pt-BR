---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48d62b1f90851025f82cd13e5d0da005b0d96ca4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35517648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsagePages = await graphClient.Reports.GetSharePointSiteUsagePages('D7')
    .Request()
    .GetAsync();

```