---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d844a43f71475d7af9128683e6d56291fce9d53d5a85c938514109d87f5e101
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingBusinesses = await client.api('/bookingBusinesses')
    .version('beta')
    .get();

```