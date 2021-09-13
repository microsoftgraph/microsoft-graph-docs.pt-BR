---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a48fb1d7ef8140af48bcc4be1efd382a98fce36f93675fa3826efd4899624235
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273471"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}/members/{member-id}')
    .delete();

```