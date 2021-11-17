---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56c2608b0626519523155a321495c1276a83d973dbd2e672e9f90bddf1825e0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Drive.Items["{driveItem-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```