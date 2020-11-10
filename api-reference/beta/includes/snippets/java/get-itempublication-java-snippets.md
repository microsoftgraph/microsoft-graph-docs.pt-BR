---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f130dd9791a49a4a7d3406e695aa4d8800449f9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952400"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPublication itemPublication = graphClient.me().profile().publications("{id}")
    .buildRequest()
    .get();

```