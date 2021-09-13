---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21e435419b6f4113e1c0c5b6ea903e95b7d089d96ef5d5411f4e278757336a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let message = await client.api('/me/messages/AAMkADhAAAW-VPeAAA=/')
    .select('internetMessageHeaders')
    .get();

```