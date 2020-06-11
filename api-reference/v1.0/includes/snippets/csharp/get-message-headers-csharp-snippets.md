---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec7039ef0ac3cff61e22d8dae8bb481818ac7da9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADhAAAW-VPeAAA="]
    .Request()
    .Select("internetMessageHeaders")
    .GetAsync();

```