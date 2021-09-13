---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 431218b3968243b5df4291f95f8ac72d94e237d43e5230d78b3911bf736c9886
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedTimeZones = await graphClient.Me.Outlook
    .SupportedTimeZones()
    .Request()
    .GetAsync();

```