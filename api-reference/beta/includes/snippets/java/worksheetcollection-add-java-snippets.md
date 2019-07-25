---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6d8e89f4ef8d7e7170d894a4c345d89bd523394
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866050"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String name = "name-value";

graphClient.me().drive().items("{id}").workbook().worksheets()
    .add(name)
    .buildRequest()
    .post();

```