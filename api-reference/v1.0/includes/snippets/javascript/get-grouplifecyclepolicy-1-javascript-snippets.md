---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 328d76f9ffd8818f9c50d3ca1f2bce9a28621622a9a16297767f70501cfa8d73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicy = await client.api('/groupLifecyclePolicies/{id}')
    .get();

```