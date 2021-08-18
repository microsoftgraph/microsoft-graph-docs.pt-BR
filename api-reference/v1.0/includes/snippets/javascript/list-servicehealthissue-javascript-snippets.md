---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b391c2c4459068c769f7a39d787c99f58ff90a91
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58260801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let issues = await client.api('/admin/serviceAnnouncement/issues')
    .get();

```