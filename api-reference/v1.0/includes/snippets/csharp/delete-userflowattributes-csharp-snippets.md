---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1adad3a18db44c785d46b5d72e972d68bae9a62b
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlowAttributes["{identityUserFlowAttribute-id}"]
    .Request()
    .DeleteAsync();

```