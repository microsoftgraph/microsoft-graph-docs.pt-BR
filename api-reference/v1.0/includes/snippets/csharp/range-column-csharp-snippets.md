---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1627621660fea5cc656795681b12e0864f004f9ba7ad861ce1bda2f3b0e30ec2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Names["{workbookNamedItem-id}"]
    .Range()
    .Column(5)
    .Request()
    .GetAsync();

```