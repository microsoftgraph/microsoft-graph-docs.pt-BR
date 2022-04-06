---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d419c6cfc6796a05cafe843721d2b7b4a9d66aa5
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Id = "123456!87"
};

await graphClient.Drive.Bundles["{driveItem-id}"].Children
    .Request()
    .AddAsync(driveItem);

```