---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5065995f6d14a53390f6a06f9854d974852091e33f9db2f02cfb5b77aea96a3d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326673"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorCollectionPage members = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").members()
    .buildRequest()
    .get();

```