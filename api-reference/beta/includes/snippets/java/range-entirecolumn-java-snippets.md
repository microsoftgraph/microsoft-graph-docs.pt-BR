---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d53c365d811fcab9cdbc33631cae013666205f24
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974458"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .entireColumn()
    .buildRequest()
    .get();

```