---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4f3c983e1d1bf1196f80be53670c3a91847674b7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952784"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .buildRequest()
    .post();

```