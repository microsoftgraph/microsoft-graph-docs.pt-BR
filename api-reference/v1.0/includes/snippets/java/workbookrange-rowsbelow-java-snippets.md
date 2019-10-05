---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e29c9e6ec1639fe4ca9eac3da8fb72a8bbb4dd0e
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402834"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id}")
    .range()
    .rowsBelow(null)
    .buildRequest()
    .post();

```