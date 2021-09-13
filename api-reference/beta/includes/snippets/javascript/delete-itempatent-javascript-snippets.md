---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1c4f651f05c48353ef4905ed7c08250d28ad88dacfd8b84d4a50e6156243056
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273321"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/patents/{id}')
    .version('beta')
    .delete();

```