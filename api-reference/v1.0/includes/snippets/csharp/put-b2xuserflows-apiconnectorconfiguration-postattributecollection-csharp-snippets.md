---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f48696b7778a5bdfc20c317bb8f591879e1c9684
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].PostAttributeCollection.Reference
    .Request()
    .PutAsync("{id}");

```