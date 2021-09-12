---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d29d853f7088ace55fa77e58dba58535b791510ed99da846c248de611124327c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .get();

```