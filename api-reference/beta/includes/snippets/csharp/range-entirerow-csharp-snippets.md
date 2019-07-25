---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85dad11757ad26d3708e2475aba3f07f9d5bea4c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874877"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRange = await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .EntireRow()
    .Request()
    .GetAsync();

```