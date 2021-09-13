---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 843622052b619fb936eb28e927e278b1810f3885e9b9f30a3ed634b8dbf585f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406845"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comments = await graphClient.Drive.Items["{driveItem-id}"].Workbook.Comments
    .Request()
    .GetAsync();

```