---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c94b8fc75c691d39e2e0a43ebf2974c7d4ec06ce
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981199"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .unmerge()
    .buildRequest()
    .post();

```