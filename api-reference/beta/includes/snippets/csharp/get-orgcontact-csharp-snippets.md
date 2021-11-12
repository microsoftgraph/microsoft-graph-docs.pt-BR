---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd8d122392c6051fc8351ac7cefb939d2d50e575f1bce101f1ba3d8701ab743b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = await graphClient.Contacts["{orgContact-id}"]
    .Request()
    .GetAsync();

```