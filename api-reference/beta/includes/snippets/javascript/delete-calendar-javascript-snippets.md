---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1e8864c7df9977afb77d2e22dcc9a88eb755684
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603320"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .delete();

```