---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44fa434585498096699c2011d1129f9ec3991676
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders')
    .get();

```