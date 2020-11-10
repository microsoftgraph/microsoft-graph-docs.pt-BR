---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec341925c5adaed5e1a48e1ae5bc269a5ed90f94
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48969726"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISiteCollectionPage sites = graphClient.sites("{site-id}").sites()
    .buildRequest()
    .get();

```