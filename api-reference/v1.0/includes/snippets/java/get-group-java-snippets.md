---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c949bf9fe6671e84da6213f99936fddf7eadc708
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35886429"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.groups("b320ee12-b1cd-4cca-b648-a437be61c5cd")
    .buildRequest()
    .get();

```