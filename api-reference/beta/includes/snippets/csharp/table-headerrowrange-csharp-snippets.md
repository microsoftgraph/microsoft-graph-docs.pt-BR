---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee049cc3613c5acf7ceb72267bebeabff8cd151ee79a5383486e4b253f953703
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159343"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables["{workbookTable-id}"]
    .HeaderRowRange()
    .Request()
    .GetAsync();

```