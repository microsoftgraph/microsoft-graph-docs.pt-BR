---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59504c66214b6c506b4add1d20abdb898412bde5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980380"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .totalRowRange()
    .buildRequest()
    .post();

```