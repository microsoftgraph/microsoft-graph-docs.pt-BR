---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0dba8560fd339f583ebd83da51885e4fa0da64bb04c3dfcf1df49f7bb15229ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let healthOverviews = await client.api('/admin/serviceAnnouncement/healthOverviews')
    .version('beta')
    .get();

```