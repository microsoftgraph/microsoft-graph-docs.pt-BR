---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4bfc7172adb61ed99b9f7d2fbc8f25a2c0e2177
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .delete();

```