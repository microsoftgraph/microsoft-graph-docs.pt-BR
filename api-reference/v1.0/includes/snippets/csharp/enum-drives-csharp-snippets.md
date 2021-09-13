---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08a4b90bcba0d717099f8cf180f1791d0d68022b0ea2268ef035f20e12d6d150
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102715"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var drives = await graphClient.Me.Drives
    .Request()
    .GetAsync();

```