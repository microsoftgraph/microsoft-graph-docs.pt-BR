---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efe03965de2a0b2affdfa1f271d972c13dd5c87d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/createdObjects')
    .get();

```