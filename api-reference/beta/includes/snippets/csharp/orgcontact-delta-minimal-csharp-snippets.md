---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8078b18e910b0f32c0823b237b47371686a79c5b5cde703b44c943d6f543f3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216708"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Contacts
    .Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select("displayName,jobTitle,mail")
    .GetAsync();

```