---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 422ea191006ea70b7dc40ec3c614a8f349ea6b69
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43511050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

let res = await client.api('/domains/{id}/forceDelete')
    .post(forceDelete);

```