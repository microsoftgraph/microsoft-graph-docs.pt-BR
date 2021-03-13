---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1159cde573d8a3b58809051d4174fd387b004fc9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/users/{idOrUserPrincipalName}/drive')
    .version('beta')
    .get();

```