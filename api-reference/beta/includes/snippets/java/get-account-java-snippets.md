---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddb56f560c3bb4622a1ed1bb465312cb56238028
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441085"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserAccountInformationCollectionPage account = graphClient.me().profile().account()
    .buildRequest()
    .get();

```