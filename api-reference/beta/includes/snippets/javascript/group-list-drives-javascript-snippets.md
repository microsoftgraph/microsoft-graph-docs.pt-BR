---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fee5562fbd5c724a294fc859a24f1ef876f2ab60bd75d1790108f55d3588fac4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/groups/{groupId}/drives')
    .version('beta')
    .get();

```