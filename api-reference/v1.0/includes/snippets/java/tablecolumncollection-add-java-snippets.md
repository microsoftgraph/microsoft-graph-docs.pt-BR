---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70136f0ca7a983dea9cd934d8ade2d4eff49bb488263202c77785b75fc9ce633
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

int index = 3;

LinkedList<JsonElement> valuesList = new LinkedList<JsonElement>();
JsonElement values = new JsonObject();

valuesList.add(values);

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns()
    .add(WorkbookTableColumnAddParameterSet
        .newBuilder()
        .withIndex(index)
        .withValues(values)
        .withName(null)
        .build())
    .buildRequest()
    .post();

```