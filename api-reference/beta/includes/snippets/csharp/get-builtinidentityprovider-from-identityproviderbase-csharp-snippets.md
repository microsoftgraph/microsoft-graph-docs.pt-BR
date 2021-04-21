---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 829261618cb3ba02837b0bcdbeef598ee04f0039
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = await graphClient.Identity.IdentityProviders["{identityProviderBase-id}"]
    .Request()
    .GetAsync();

```