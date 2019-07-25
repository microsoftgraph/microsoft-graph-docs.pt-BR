---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24ea5c405f77150715d195785a0707a030c4a18a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861660"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("contoso.com")
    .verify()
    .buildRequest()
    .post();

```