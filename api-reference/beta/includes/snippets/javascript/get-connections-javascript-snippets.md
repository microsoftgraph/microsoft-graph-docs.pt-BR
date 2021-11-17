---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a9d4f066c13f45ca67e679a397ac8d971fa834c183e4aa31af7c910a7ef6618
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connections = await client.api('/external/connections')
    .version('beta')
    .get();

```