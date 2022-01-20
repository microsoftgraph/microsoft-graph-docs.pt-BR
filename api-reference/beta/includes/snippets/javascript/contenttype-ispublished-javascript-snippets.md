---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b724b212f1534174a3eb4283749bb5f1f5e4a43dc83aa7702e48385b3569c989
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let _boolean = await client.api('/sites/{siteId}/contentTypes/{contentTypeId}/isPublished')
    .version('beta')
    .get();

```