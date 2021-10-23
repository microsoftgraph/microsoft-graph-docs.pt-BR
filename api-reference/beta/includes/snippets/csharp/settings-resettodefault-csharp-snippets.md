---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eeea6d9e5bec9d074af572b8f742a049360570bd474d4abbf9324afcd8f538b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157237"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].Settings
    .ResetToDefault()
    .Request()
    .PostAsync();

```