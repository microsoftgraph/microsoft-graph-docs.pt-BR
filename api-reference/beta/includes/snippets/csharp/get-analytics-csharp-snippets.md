---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab80c472adb80a248eba014ae7867234b0d8c6e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802562"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAnalytics = await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"].Analytics
    .Request()
    .GetAsync();

```