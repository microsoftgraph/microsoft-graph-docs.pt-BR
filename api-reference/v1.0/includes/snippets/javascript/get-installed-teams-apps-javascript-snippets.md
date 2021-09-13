---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bbae5c50ffbf32c5079c229d48d5a678f2934d84673715263175f3cdf507cb2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsAppInstallation = await client.api('/teams/{id}/installedApps/{id}')
    .get();

```