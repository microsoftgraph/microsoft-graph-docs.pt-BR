---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a846619669d9b9452cffcf0fede4022ad93221ea769dc1483b819436052eacb8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .DeleteAsync();

```