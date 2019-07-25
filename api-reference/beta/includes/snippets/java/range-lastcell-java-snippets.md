---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b582272c2adbedb2c933348c66dd0d7860245ce8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874816"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastCell()
    .buildRequest()
    .get();

```