---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbf2a21e94e3ecde9808cab87adc9364d02745d8640f2c067e592895ddec8a64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var replies = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments["{workbookComment-id}"].Replies
    .Request()
    .GetAsync();

```