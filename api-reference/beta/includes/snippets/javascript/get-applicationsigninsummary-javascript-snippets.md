---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f0b2da742150300faa6c75bc3d6a24307b51b02fd70efcb43217a5412d9b1eca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAzureADApplicationSignInSummary = await client.api('/reports/getAzureADApplicationSignInSummary(period='D7')')
    .version('beta')
    .get();

```