---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e782c695390483fbbd81c479b14c9d6baa283975
ms.sourcegitcommit: af9489bd42a25dff04836dcfcc57369259fda587
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2022
ms.locfileid: "66577925"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.customRequest("/reports/getM365AppUserDetail(period='D7')", InputStream.class)
    .buildRequest()
    .get();

```