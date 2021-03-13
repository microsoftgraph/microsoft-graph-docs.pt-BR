---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38dbf786a00529c9db6139d8cc871fe2f0d01965
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printConnector = {
  name: 'ConnectorName',
  fullyQualifiedDomainName: 'CONNECTOR-MACHINE',
  operatingSystem: 'Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555',
  appVersion: '0.19.7338.23496',
  location: {
    latitude: 1.1,
    longitude: 2.2,
    altitudeInMeters: 3
  }
};

await client.api('/print/connectors/{id}')
    .version('beta')
    .update(printConnector);

```