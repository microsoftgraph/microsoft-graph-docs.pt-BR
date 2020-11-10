---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34aab3d1def0aba64b2dabbf8a079827fed43d2b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980282"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IListCollectionPage lists = graphClient.sites("{site-id}").lists()
    .buildRequest()
    .get();

```