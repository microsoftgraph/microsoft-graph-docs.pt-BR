---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98b03755515b56c1167f479c3a20e284476cff4e90a327cd143d822c4b0cfcd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275649"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Schools["{educationSchool-id}"].Classes["{educationClass-id}"]
    .Request()
    .DeleteAsync();

```