---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff8a120c3217424039758a7c965b8c940c7231be
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893525"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityPages('D7')
    .buildRequest()
    .get();

```