---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c7145e8e7ec18143d63f75c2a40df28aa9f0f6738521fbb0888fbbf6c06f03d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let driveItem = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .version('beta')
    .get();

```