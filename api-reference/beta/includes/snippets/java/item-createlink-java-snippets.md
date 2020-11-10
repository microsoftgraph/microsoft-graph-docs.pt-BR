---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6b77b4da98b8c209866285cdca0febca1894001
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963875"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String type = "view";

String password = "ThisIsMyPrivatePassword";

String scope = "anonymous";

graphClient.me().drive().items("{itemId}")
    .createLink(type,scope,null,password,null,null)
    .buildRequest()
    .post();

```