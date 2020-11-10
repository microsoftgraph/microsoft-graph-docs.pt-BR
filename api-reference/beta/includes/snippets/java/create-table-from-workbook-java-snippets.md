---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1644c25b258ef9582c72bbfc1c4a9455d73e465d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977574"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "A1:D8";

Boolean hasHeaders = false;

graphClient.me().drive().items("{id}").workbook().tables()
    .add(address,hasHeaders)
    .buildRequest()
    .post();

```