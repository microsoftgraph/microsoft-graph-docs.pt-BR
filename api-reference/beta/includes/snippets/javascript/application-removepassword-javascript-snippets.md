---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11db73c436ae6ce93a24506c02425ca3cced2638
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37994944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removePassword = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6"
};

let res = await client.api('/applications/{id}/removePassword')
    .version('beta')
    .post(removePassword);

```