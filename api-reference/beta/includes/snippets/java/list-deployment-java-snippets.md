---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d99a685f0634ce9ed12e144dcb4b48767c34411ccaf25cc97e2ed4b165f43409
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DeploymentCollectionPage deployments = graphClient.admin().windows().updates().deployments()
    .buildRequest()
    .get();

```