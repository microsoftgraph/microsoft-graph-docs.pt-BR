---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5cdc34fde8640fb8fc47807854377720e1de731e0516be2a68d3ee503e163952
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216971"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var labels = await graphClient.Me.InformationProtection.Policy.Labels
    .Request()
    .GetAsync();

```