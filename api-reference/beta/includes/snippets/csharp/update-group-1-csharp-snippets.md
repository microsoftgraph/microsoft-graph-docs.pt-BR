---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10addcd2a38f6982a9fb365392f4d425786c9dff396252d5193798b1c951e800
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272682"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Contoso Life v2.0",
    DisplayName = "Contoso Life Renewed"
};

await graphClient.Groups["{group-id}"]
    .Request()
    .UpdateAsync(group);

```