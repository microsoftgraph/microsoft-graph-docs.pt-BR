---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80a86b481412bf958a376a6ea8b214858a6f05456fb0d0a7cfbe5a05af41ebe3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216068"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamCollectionPage joinedTeams = graphClient.me().joinedTeams()
    .buildRequest()
    .get();

```