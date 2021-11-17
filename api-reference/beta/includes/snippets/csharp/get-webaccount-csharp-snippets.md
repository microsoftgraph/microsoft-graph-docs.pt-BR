---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d23442943fa3a33a9cfc8abccb7ac15d53e32a790badc11f81d3086bcdd865b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159884"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var webAccount = await graphClient.Me.Profile.WebAccounts["{webAccount-id}"]
    .Request()
    .GetAsync();

```