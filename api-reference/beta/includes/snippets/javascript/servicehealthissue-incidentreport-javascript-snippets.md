---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: deda391f27c49481c1f448fa673958dca865f7a042b1d7111b62a438a0b0b365
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101956"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/admin/serviceAnnouncement/issues/MO248163/incidentReport')
    .version('beta')
    .get();

```