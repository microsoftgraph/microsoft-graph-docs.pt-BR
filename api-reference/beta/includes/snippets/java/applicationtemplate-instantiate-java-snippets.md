---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9e49ce56f00b8412c127a2fbd5f9d0f5f5f076e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856687"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "My custom name";

graphClient.applicationTemplates("{id}")
    .instantiate(displayName)
    .buildRequest()
    .post();

```