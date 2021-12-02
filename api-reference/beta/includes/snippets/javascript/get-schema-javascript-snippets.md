---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6116e1f2a9ee9656d1b5b59a795fd8cf6b60e1804ffab8ae5b230e43a080033a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/external/connections/contosohr/schema')
    .version('beta')
    .get();

```