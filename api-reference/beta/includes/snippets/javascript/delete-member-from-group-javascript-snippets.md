---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0b2e80cd7428ff96f934be7eadf580a97e005f989279d795ae528d8ccd681d1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{group-id}/members/{directory-object-id}/$ref')
    .version('beta')
    .delete();

```