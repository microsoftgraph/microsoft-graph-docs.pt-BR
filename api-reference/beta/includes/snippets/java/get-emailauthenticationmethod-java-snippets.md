---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3dd5725020d2e35317b613bca5e0cdeed2cae887
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955094"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailAuthenticationMethodCollectionPage emailMethods = graphClient.me().authentication().emailMethods()
    .buildRequest()
    .get();

```