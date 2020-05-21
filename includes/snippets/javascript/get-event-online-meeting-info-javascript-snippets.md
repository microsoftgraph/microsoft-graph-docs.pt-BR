---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5b8dd4a1d56cef296258acb6227fa09d5dd3025
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkADAGu0AABIGYDZAAA=')
    .select('isOnlineMeeting,onlineMeetingProvider,onlineMeeting')
    .get();

```