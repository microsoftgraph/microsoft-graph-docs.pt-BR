---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6d8e89f4ef8d7e7170d894a4c345d89bd523394
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979960"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets()
    .add(name)
    .buildRequest()
    .post();

```