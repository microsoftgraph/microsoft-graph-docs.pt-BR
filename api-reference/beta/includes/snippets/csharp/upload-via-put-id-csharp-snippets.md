---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 653c64ae73f410f3a67e9d554b00a9c273655b30
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes(@"The contents of the file goes here."));

await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request()
    .PutAsync<DriveItem>(stream);

```