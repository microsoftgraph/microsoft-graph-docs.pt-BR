---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2732d023798b4af955503939406d485fd104fef7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryroles/{id}/members/{id}/$ref')
    .version('beta')
    .delete();

```