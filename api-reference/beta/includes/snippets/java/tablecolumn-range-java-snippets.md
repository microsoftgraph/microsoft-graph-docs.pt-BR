---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4ba54538fb0c5b49494422e49c0e80fde79e1c963820fe696af7b2fd2bb446e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159049"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .range()
    .buildRequest()
    .get();

```