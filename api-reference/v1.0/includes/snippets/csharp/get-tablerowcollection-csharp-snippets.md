---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df04b60477716cfd6ca2768165c5d2692a8167d892b87739492747a2d083f7aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rows = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"].Rows
    .Request()
    .GetAsync();

```