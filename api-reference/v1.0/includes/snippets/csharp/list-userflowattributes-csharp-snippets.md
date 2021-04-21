---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 344ac93cefa49cc17101552254c6a45bbe0a2f34
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userFlowAttributes = await graphClient.Identity.UserFlowAttributes
    .Request()
    .GetAsync();

```