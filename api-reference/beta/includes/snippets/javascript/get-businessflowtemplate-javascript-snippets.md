---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c86a4a9dd6d2211040aacc95469f565071bb7e7a33593219cd18dfdc7bdd5e05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let businessFlowTemplates = await client.api('/businessFlowTemplates')
    .version('beta')
    .get();

```