---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5c039f1cb10959ad7f96131f8d9d900e9ed83421cc6b466337c6a0dbee84b5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let linkedResource = await client.api('/me/todo/lists/dfsdc-f9dfdfs-dcsda9/tasks/e2dc-f9cce2-dce29/linkedResources/f9cddce2-dce2-f9cd-e2dc-cdf9e2dccdf9')
    .version('beta')
    .get();

```