---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79acc987a9a110e182158fe580ef059c4c43cdad1fdc83bcbcd56e6dfb6bed7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214480"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkBot teamworkBot = graphClient.appCatalogs().teamsApps("e4c5c249-bb4b-419e-b7c5-b1d98559368b").appDefinitions("ZTRjNWMyNDktYmI0Yi00MTllLWI3YzUtYjFkOTg1NTkzNjhiIyMyLjAuMSMjUHVibGlzaGVk").bot()
    .buildRequest()
    .get();

```