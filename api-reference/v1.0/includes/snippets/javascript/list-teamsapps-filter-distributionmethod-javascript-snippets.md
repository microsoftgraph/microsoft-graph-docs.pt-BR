---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67988aaffb0a3e4a79b6b4b236f00e87bff76f61cae45fe44e564afabaf7c526
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .filter('distributionMethod eq \'organization\'')
    .get();

```