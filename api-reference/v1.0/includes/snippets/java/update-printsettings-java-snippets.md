---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efb09cbb7300b15152e6f367dd96bf9fd3f1f06e2172dc92f6832eea335dcbfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273106"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintSettings printSettings = new PrintSettings();
printSettings.documentConversionEnabled = true;

graphClient.customRequest("/print/settings", PrintSettings.class)
    .buildRequest()
    .patch(printSettings);

```