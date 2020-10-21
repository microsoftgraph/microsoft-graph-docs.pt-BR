---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad4cb296e95947f0081d7c77059ab85e7a13cea1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/dismissReminder')
    .post();

```