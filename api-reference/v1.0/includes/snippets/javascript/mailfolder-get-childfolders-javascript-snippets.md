---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1d6573b76cba36910e8ba65bf5eba2e8f8f6182044dbdb2dbdf1935320a46c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let childFolders = await client.api('/me/mailFolders/{id}/childFolders')
    .get();

```