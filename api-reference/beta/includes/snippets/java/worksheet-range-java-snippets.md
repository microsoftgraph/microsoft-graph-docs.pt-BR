---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9016ca5dec075220f8f31a11b2fc832b627f4236
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444568"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WorkbookRange workbookRange = graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .range()
    .buildRequest()
    .get();

```