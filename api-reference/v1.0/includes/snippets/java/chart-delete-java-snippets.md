---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf209225773ea452180837ffa268c5fcdd45dc54b6f40696788bc581cfef6151
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}").charts("{name}")
    .buildRequest()
    .delete();

```