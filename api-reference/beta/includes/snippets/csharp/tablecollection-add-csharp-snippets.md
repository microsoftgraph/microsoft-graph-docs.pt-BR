---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d44970c141a83341738a7afda68052b5458d257c597e1a8e9804e065bb60ebfe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157975"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var address = "Sheet1!A1:D5";

var hasHeaders = true;

await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Add(hasHeaders,address)
    .Request()
    .PostAsync();

```