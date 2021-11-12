---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6f7ebdafbeaa74cb8acc9dad3aad1efde8522b481d9623bdbae03b5083a079e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217286"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calculationType = "calculationType-value";

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Application
    .Calculate(calculationType)
    .Request()
    .PostAsync();

```