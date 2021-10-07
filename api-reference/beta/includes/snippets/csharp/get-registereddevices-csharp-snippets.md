---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 347ed3650a6f111d6b19f6d5af6968ca9ec07ef3777e73353dcd8ed8d89b2ef9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329358"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredDevices = await graphClient.Me.RegisteredDevices
    .Request()
    .GetAsync();

```