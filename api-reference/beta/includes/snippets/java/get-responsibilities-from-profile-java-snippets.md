---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 520aba2b2c49e60a72b7925bbded12565f9937ac
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441039"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IStringCollectionPage responsibilities = graphClient.customRequest("/me/responsibilities", IStringCollectionPage.class)
    .buildRequest()
    .get();

```