---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 284cfdab73ec319383a49352a484693677b358a98bb8b391c4753c500593f550
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/teams/{id}/channels/{id}/filesFolder')
    .version('beta')
    .get();

```