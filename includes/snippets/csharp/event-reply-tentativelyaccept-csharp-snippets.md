---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cee6e70c844920fa77502ebc4555b2669ea6ae522226df152fe66a74f99eb487
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "I will probably be able to make it.";

var sendResponse = true;

await graphClient.Me.Events["AAMkADADVj3fyAABZ5ieyAAA="]
    .TentativelyAccept(comment,sendResponse)
    .Request()
    .PostAsync();

```