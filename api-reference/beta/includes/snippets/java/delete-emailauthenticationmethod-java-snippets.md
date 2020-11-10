---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3694edf759ee4687b8671555f7308528651dd61b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955119"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("kim@contoso.com").authentication().emailMethods("3ddfcfc8-9383-446f-83cc-3ab9be4be18f")
    .buildRequest()
    .delete();

```