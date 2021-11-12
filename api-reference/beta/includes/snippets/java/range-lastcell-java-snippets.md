---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02ce3aa7cfac70b5dccf4e730061a94582f87e06ecb2c7a5fffc529a2d1b0944
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214729"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastCell()
    .buildRequest()
    .get();

```