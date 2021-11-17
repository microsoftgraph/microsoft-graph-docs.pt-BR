---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 034a180d8a8a5a5c92e160f0f1b41c1ec7f42457fe4551b045218fa45d0b518f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899274"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceUpdateMessage = await client.api('/admin/serviceAnnouncement/messages/MC172851')
    .version('beta')
    .get();

```