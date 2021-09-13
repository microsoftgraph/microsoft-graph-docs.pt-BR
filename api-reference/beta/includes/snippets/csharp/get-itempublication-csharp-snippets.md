---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b3c046d3d130dd00ac5e28a50363e673cae7d74c8bfc4e0bac04acc21a68d76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217603"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = await graphClient.Me.Profile.Publications["{itemPublication-id}"]
    .Request()
    .GetAsync();

```