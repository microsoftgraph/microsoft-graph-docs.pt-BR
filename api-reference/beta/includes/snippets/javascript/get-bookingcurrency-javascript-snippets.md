---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 487c9accc48f3d84d4fc4df8d3aa0927caa0c1bb45f349f2b94d5462d13e4b26
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCurrency = await client.api('/bookingCurrencies/USD')
    .version('beta')
    .get();

```