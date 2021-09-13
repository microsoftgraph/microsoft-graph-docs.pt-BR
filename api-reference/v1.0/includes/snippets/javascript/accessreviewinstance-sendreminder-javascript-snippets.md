---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a1a731cc55a96f37b3ce4aa19f27dc11ba300bb666bf3c068701203b5141b1a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/accessReviews/definitions/8564a649-4f67-4e09-88e7-55def6530e88/instances/1234a649-4f67-1234-88e7-55def6530e88/sendReminder')
    .post();

```