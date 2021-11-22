---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9e049af6d71e647faf4e91fcd32b5c3718219eb27749437ef6975aea6b7efd0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327104"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.SynchronizationProfiles["{educationSynchronizationProfile-id}"]
    .Request()
    .DeleteAsync();

```