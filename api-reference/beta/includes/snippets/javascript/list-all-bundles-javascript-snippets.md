---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f87731d03972656d7d85b406968fadac4062b0bdc9b57f08ab6a1d03329ffc0d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bundles = await client.api('/drive/bundles')
    .version('beta')
    .get();

```