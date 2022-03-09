---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbd38445bb95f155dcc3cf3a9e0f8018e6a39682
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394275"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extensionProperty = await graphClient.Applications["{application-id}"].ExtensionProperties["{extensionProperty-id}"]
    .Request()
    .GetAsync();

```