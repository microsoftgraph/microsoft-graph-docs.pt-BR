---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b2f7e7d35804bbf86ad4b432892e1a19818fce16
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2021
ms.locfileid: "60560855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmissionResource = {
    resource: {
        displayName: 'category.jpg',
        fileUrl: 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG',
        '@odata.type': '#microsoft.graph.educationMediaResource'
    }
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/submissions/da443246-384d-673b-32db-bdba9d7f2b51/resources')
    .version('beta')
    .post(educationSubmissionResource);

```