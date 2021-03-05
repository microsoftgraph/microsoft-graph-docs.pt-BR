---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34b6d413f6db75a0537317feef78fc2be2988162
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475799"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassMethods = await graphClient.Me.Authentication.TemporaryAccessPassMethods
    .Request()
    .GetAsync();

```