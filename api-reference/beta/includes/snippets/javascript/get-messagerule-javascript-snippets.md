---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0047509bd1264f21aecaccd5f3ce08aeec3bd406a93e26289836975df756ac25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRule = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .get();

```