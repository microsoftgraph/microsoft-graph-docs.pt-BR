---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 96c9f24678bc4fc20acf51663b9744ce19ab83d6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968203"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintService printService = graphClient.print().services("{id}")
    .buildRequest()
    .get();

```