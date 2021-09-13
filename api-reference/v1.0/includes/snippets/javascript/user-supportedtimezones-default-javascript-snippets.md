---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 083808081836d6539ef2b49cb9fbbfc3d9c9e486f70f0ecd2524c86179709cc1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216635"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedTimeZones = await client.api('/me/outlook/supportedTimeZones')
    .get();

```