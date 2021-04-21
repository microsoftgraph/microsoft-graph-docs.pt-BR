---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a94a878af011fb2cdeac5460e90ca6fcfeb3ab91
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921377"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityProviderBaseCollectionPage identityProviders = graphClient.identity().identityProviders()
    .buildRequest()
    .get();

```