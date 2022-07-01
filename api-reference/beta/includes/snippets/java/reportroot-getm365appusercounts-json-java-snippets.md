---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 961f10576d5eb20988c2dad50aef6e576ba1c8cc
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577902"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppUserCounts(period='D7')", InputStream.class)
    .buildRequest()
    .get();

```