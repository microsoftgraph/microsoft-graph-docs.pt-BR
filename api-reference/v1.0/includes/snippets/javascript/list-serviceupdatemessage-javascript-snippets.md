---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 111923e9dd74440885883357a59f4c89d56871c8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58256938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/admin/serviceAnnouncement/messages')
    .get();

```