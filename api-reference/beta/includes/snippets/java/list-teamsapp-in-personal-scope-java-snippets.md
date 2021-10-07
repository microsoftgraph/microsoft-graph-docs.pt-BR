---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd944cb4d6f7370506c65113d8bb5478021583d23048614de3a6ace7f63e8c46
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213667"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("appDefinitions/any(a:a/allowedInstallationScopes has 'personal')")
    .expand("appDefinitions($select=id,displayName,allowedInstallationScopes)")
    .get();

```