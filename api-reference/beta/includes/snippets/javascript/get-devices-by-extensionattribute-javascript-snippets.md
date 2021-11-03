---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db8b3cb486da5ed8f80eac6d132e18dbfba9bb01
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60694547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let devices = await client.api('/devices')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('extensionAttributes/extensionAttribute1 eq \'BYOD-Device\'')
    .get();

```