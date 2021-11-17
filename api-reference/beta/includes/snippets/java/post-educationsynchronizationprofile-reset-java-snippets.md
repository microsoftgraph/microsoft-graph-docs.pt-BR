---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df3926b2f7b4906478e9c5669763b9e927db5c92e28c5928d6a478cd96470192
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100463"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().synchronizationProfiles("{id}")
    .reset()
    .buildRequest()
    .post();

```