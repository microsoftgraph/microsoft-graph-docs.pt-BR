---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2c0d0b4ca0037d8535739245fe4cab137fee0b8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968495"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .delete();

```