---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b72c0d4ce215d90e1d524a0e95bd02374ab9c494
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')')
    .version('beta')
    .delete();

```