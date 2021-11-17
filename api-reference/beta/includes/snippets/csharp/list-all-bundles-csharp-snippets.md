---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4070baecbd856f5e13d50efb17a28d17f9985b9f736efff316583ef13c68e6e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bundles = await graphClient.Drive.Bundles
    .Request()
    .GetAsync();

```