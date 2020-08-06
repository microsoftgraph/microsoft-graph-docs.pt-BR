---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8949cb73facf7f06951d4516878d49593c3998be
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567025"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookOperation workbookOperation = graphClient.me().drive().items("{drive-item-id}").workbook().operations("{operation-id}")
    .buildRequest()
    .get();

```