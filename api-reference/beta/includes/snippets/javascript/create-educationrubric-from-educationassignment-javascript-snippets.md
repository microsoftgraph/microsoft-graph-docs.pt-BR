---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6070d5d8a68dc5f20c572246669eb18bd813b09fa3c97173776962328747867
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/education/me/rubrics/{id}'
};

await client.api('/education/classes/{id}/assignments/{id}/rubric/$ref')
    .version('beta')
    .put(educationRubric);

```