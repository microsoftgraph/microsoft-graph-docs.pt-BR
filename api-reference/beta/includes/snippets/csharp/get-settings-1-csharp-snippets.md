---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33188b07da4d0cd4a356ebcc196947d30286b05f8a0e531cc7b14b1d4a7ba598
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328065"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Settings
    .Request()
    .GetAsync();

```