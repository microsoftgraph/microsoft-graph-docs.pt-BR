---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f3e27e82a250674899ddf1adb024898edb99467
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10001')
    .version('beta')
    .get();

```