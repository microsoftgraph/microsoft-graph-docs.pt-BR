---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 479aa7ac4f98fd49a1609558c3d7502104dfd02112e44a8e5d33e9eff2981186
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessReviewReviewer = {
    id: '006111db-0810-4494-a6df-904d368bd81b'
};

await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers')
    .version('beta')
    .post(accessReviewReviewer);

```