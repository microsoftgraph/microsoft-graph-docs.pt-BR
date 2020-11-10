---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 879a36fa33804c4b7fbd6507e8fbc61d254a85f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973674"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format()
    .autofitRows()
    .buildRequest()
    .post();

```