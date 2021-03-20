---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6755864dcb0a28ab11a3e4031e5bb867d97223ae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951130"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationUser = await client.api('/education/users/13012')
    .version('beta')
    .get();

```