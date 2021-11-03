---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d81ff043a02b7c826c469904295a648020409c5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694546"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .version('beta')
    .select('id,extensionAttributes')
    .get();

```