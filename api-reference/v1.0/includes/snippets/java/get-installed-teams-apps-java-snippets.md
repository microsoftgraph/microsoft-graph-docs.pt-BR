---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a78152f0e54b515d77cb69408f0cd7618d24d2b5d6bd056a2bb98a57328a3495
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273079"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .get();

```