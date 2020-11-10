---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9204c501fd49fbdb6b661301b1608a507b99a78
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981888"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRangeBorder workbookRangeBorder = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().borders("{sideIndex}")
    .buildRequest()
    .get();

```