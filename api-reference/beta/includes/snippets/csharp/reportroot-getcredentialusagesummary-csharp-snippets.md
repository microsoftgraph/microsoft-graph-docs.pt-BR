---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eeac8c70c8c308aeb1d09c2c5c6abfb461b807c992654597d44157064cb6e221
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getCredentialUsageSummary = await graphClient.Reports
    .GetCredentialUsageSummary("D30")
    .Request()
    .Filter("feature eq 'registration'")
    .GetAsync();

```