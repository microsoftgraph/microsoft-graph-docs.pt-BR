---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 223959ba3f985ae7cb601e52d7902af3e55961995903477b0a5f2efe33d70eaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .DeleteAsync();

```