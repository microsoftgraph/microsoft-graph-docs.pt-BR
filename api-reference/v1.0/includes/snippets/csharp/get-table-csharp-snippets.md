---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78ccd162389f82b279b322fbbc0c855f17d36d0ce4e5efbe1c77c9f06f10c747
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376661"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookTable = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .Request()
    .GetAsync();

```