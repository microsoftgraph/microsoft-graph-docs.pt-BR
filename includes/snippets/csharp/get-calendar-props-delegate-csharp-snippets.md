---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b3bc87a8fe392e4da5db3e9d85f2d94d6ace64602ff75f46054c2373700dbed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237012"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var calendar = await graphClient.Users["meganb@contoso.OnMicrosoft.com"].Calendars["AAMkADlAABhbftjAAA="]
    .Request()
    .GetAsync();

```