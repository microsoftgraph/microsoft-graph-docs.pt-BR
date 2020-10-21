---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2e6aeb839929f019d81d4d8bae77d045a50fa87
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedDevices')
    .get();

```