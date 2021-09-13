---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2898a4d2734507fc696edbe547542e6a9e822324e0db4208cb3e9364d7141556
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tables = await graphClient.Me.Drive.Items["{driveItem-id}"].Workbook.Tables
    .Request()
    .GetAsync();

```