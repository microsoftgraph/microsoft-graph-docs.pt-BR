---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 196055f00bcc63cdab721e2f8fb31be6268401c2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433495"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().account("{id}")
    .buildRequest()
    .delete();

```