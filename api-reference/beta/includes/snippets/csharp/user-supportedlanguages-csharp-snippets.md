---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fa68ecd8f206a13381f77dce1558b49f4e2d42091952ae11a9558050a502a70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271931"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var supportedLanguages = await graphClient.Me.Outlook
    .SupportedLanguages()
    .Request()
    .GetAsync();

```