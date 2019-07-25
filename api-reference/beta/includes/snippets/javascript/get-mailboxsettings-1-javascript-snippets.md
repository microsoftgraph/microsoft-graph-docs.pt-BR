---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1c50c164319b4b9a1e39f7dfeef2696fff2555d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings')
    .version('beta')
    .get();

```