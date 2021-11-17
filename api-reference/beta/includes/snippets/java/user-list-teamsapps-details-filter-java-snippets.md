---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca394a10ecefd8222fec9a49f1cc68978cb7a786ad67410bcc4f34e3e72f2ece
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159746"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("97a5a533-833d-494b-b543-c0afe026cb96").teamwork().installedApps()
    .buildRequest()
    .filter("teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'")
    .expand("teamsAppDefinition")
    .get();

```