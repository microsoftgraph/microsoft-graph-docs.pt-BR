---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05be4557a8dafe253f67dc0e91dc8825b22938cf4b4ea31a2b439f04ae37c148
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let createdObjects = await client.api('/servicePrincipals/{id}/createdObjects')
    .version('beta')
    .get();

```