---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52b34338e9d1cfa761d96a60b4d07ee9f12c150eed11cba7b71bcc035dfa3051
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows["{workbookTableRow-id}"]
    .Range()
    .Request()
    .GetAsync();

```