---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71428b732183885192cc7fe73750251529c212c6
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38710278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/accessReviews')
    .version('beta')
    .filter('businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'')
    .get();

```