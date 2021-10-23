---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae82f7c82823b9476142749aef3eabdd9a1aa876
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562731"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().root().workbook().worksheets("{id|name}").pivotTables()
    .refreshAll()
    .buildRequest()
    .post();

```