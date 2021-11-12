---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31a22b25ce370703a9904acc1785e90e1146094e99256a84d57835b67e286e2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OutlookTaskFolder outlookTaskFolder = new OutlookTaskFolder();
outlookTaskFolder.name = "Charity work";

graphClient.me().outlook().taskFolders("AAMkADIyAAAhrbPWAAA=")
    .buildRequest()
    .patch(outlookTaskFolder);

```