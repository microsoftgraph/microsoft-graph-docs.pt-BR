---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b50e6b5b8dfc4509f48a510bea5f11783a6e266e6323c591111f36aa4089ef24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214922"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = "shift-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Delete(shift)
    .Request()
    .PostAsync();

```