---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2559bba2d45472cef74310dc1710346b504668d6a652ec3c7e70ded972bf6945
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157947"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Bundles["{driveItem-id}"].Children["{driveItem-id}"]
    .Request()
    .DeleteAsync();

```