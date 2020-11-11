---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0b287acded1b651a5bc9282f67e28e95079817e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int index = 3;

LinkedList<JsonElement> valuesList = new LinkedList<JsonElement>();
JsonElement values = new JsonObject();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(index,values,null)
    .buildRequest()
    .post();

```