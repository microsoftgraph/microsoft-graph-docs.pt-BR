---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d53c365d811fcab9cdbc33631cae013666205f24
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857092"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .entireColumn()
    .buildRequest()
    .get();

```