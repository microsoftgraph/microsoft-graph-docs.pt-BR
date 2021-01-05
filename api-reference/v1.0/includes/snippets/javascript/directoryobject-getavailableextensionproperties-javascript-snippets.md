---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38fb62e8a1569e90999d53aad4b66a1e4015e8fa
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
  isSyncedFromOnPremises: "Boolean"
};

let res = await client.api('/directoryObjects/getAvailableExtensionProperties')
    .post(extensionProperty);

```