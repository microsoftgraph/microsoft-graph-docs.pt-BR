---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e13317d71cd9de797140784980ad2e44e2d8462a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971093"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .post();

```