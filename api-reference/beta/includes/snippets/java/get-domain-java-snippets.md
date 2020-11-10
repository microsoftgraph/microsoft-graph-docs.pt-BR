---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3b6fcd30b3bf0472d46f12ffe5cc883753cb85e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956019"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Domain domain = graphClient.domains("contoso.com")
    .buildRequest()
    .get();

```