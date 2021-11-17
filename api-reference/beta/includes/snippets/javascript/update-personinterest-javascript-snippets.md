---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2b876ec3be5e904d666a4a2bac3d30b02acd3ecade1c9cdab153241dff89ba5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    'Sports'
  ]
};

await client.api('/me/profile/interests/{id}')
    .version('beta')
    .update(personInterest);

```