---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9285cf5b79d6e18a8937b750a634715a6c2db345504afa5f2eef191d7bc3639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156639"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .reapplyFilters()
    .buildRequest()
    .post();

```