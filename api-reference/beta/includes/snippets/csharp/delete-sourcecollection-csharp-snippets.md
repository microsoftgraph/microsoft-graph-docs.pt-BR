---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50c15e90f5e4477cbc53314f9588d6a06c15f5bd4488acf0de9203b8ce57a497
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].SourceCollections["{ediscovery.sourceCollection-id}"]
    .Request()
    .DeleteAsync();

```