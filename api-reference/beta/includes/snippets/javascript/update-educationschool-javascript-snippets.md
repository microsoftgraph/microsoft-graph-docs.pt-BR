---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff91a3d753c7d7473b6bf7c5b74bb598b71c7ca064af2aacdcc1b55959667334
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: 'Fabrikam Arts High School',
  description: 'Magnate school for the arts. Los Angeles School District'
};

await client.api('/education/schools/10002')
    .version('beta')
    .update(educationSchool);

```