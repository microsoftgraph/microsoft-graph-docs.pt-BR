---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b769552d0b9b860d4a6aa802b799411d15318708
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466023"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Fill
    .Clear()
    .Request()
    .PostAsync();

```