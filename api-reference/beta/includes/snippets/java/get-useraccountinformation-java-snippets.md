---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 572324fdf7e9dd49ffa136a7fa6f048c3a35d435
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserAccountInformation userAccountInformation = graphClient.me().profile().account("{id}")
    .buildRequest()
    .get();

```