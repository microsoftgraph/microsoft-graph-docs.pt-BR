---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd2c14a91c542acd5b47b673fe8cf6256b07992b335461e185971847a5211476
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327209"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .ClearFilters()
    .Request()
    .PostAsync();

```