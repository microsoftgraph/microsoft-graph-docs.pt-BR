---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 686f9d815c6a5f9dde9fcf90224feda719391a37f6e7110cddcd51d8f0025d45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327004"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var classes = await graphClient.Education.Classes
    .Request()
    .GetAsync();

```