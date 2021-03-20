---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6578f0872292b922653c247b622599a3a393f20d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/sendReminder')
    .version('beta')
    .post();

```