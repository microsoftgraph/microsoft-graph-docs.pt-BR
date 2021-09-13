---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88b632320bca1fb5939b64eb87234fd6b973a6243bd577ec668e2dde95f90c09
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273080"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .expand('teamsAppDefinition')
    .get();

```