---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3be3fc2370abf3f47cca841985a8659a2cfc153984ca788aed036a6188ac8310
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range().Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```