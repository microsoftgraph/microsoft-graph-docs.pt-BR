---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5cf676c3da1dc6999209e0e01314b01bf2e0607
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printerShares/{id}/allowedUsers/{id}/$ref')
    .version('beta')
    .delete();

```