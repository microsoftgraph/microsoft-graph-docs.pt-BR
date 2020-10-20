---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f005c10702e009eafbc035f3b1d2147beca143ae
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .expand('children')
    .get();

```