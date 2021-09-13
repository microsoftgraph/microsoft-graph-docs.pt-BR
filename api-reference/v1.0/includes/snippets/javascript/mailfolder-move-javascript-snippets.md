---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4811631e67e4626e7812dd51e94d00692bc49c6692fad5fd015557e2bceee3b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: 'destinationId-value'
};

await client.api('/me/mailFolders/{id}/move')
    .post(mailFolder);

```