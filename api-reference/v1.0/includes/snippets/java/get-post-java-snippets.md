---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b380f27797a68847452f95c44f36609efccc0443
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886968"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = graphClient.groups("{id}").threads("{id}").posts("{id}")
    .buildRequest()
    .get();

```