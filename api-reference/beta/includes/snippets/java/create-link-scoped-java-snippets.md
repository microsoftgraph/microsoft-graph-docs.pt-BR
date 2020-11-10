---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26a7d7c333eb057c99cd635833c1d40d78edca64
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963877"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "edit";

String scope = "organization";

graphClient.me().drive().items("{item-id}")
    .createLink(type,scope,null,null,null,null)
    .buildRequest()
    .post();

```