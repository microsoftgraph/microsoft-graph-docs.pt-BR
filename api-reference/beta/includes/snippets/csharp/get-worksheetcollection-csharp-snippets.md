---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87984acdafb4de86b7d0af4b729c98a0317a6898a7c115ec901daae6e61f82d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```