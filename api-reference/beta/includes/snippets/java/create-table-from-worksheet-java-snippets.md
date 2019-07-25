---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91b2b72908afeb30090cd833cd49101cf4ee644b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866141"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String address = "";

boolean hasHeaders = False;

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").tables()
    .add(address,hasHeaders)
    .buildRequest()
    .post();

```