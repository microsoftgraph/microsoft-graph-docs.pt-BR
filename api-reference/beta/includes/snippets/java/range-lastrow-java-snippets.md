---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4b2b5508b3b89a350ac3e81690913837961cc18
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874735"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastRow()
    .buildRequest()
    .get();

```