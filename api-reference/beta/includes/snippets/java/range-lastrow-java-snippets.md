---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4b2b5508b3b89a350ac3e81690913837961cc18
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968093"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastRow()
    .buildRequest()
    .get();

```