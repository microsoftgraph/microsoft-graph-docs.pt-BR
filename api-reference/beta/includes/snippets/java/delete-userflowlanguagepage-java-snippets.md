---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 769285a07af66304ea4f6bc378249f5bdd89604d571c190ad166df869ab4fe01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275213"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").overridesPages("phonefactor").content()
    .buildRequest()
    .delete();

```