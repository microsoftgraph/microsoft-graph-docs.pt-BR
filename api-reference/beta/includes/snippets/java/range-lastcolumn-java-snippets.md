---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd0859fa11ec1207c92ba324e428896c2c311578
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976588"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range()
    .lastColumn()
    .buildRequest()
    .get();

```