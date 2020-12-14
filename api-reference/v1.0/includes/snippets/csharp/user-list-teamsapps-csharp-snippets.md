---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b006d68efda796e5bc1fc9a0106139821847e166
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["5b649834-7412-4cce-9e69-176e95a394f5"].Teamwork.InstalledApps
    .Request()
    .GetAsync();

```