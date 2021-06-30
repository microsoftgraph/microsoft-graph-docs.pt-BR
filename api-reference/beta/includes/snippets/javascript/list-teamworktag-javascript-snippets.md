---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74ce9b5ad6f47f038b7e98997017fd588b553204
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tags = await client.api('/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags')
    .version('beta')
    .get();

```