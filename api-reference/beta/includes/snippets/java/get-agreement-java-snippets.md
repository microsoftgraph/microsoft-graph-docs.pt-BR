---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e66cc8c4837ed58f2e082cf7296ea07c0d4cbbbe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962468"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = graphClient.agreements("{id}")
    .buildRequest()
    .expand("files")
    .get();

```