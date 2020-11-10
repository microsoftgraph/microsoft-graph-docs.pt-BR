---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73cbd0de4b2381ad554aa1415d5f1bed44aa7f6b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48973955"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .get();

```