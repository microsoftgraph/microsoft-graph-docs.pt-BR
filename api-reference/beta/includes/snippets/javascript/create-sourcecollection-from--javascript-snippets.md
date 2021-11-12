---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 934d5476e99a371dc9a31aab8bd774491e7af76c25472103623cb8c3df27498e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327962"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sourceCollection = {
    displayName: 'Quarterly Financials search',
    contentQuery: 'subject:\'Quarterly Financials\'',
    'custodianSources@odata.bind': [
        'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735'
    ]
};

await client.api('/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections')
    .version('beta')
    .post(sourceCollection);

```