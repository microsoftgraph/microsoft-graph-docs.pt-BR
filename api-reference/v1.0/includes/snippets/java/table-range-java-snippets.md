---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd7ae6909547435b2ed2b5003f91f93076c2ab36
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806091"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .range()
    .buildRequest()
    .get();

```