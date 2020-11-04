---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 763e3140b877be5bb62dec6f504f2f4c8b94b5f6
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905791"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CertificateBasedAuthConfiguration certificateBasedAuthConfiguration = new CertificateBasedAuthConfiguration();
LinkedList<CertificateAuthority> certificateAuthoritiesList = new LinkedList<CertificateAuthority>();
CertificateAuthority certificateAuthorities = new CertificateAuthority();
certificateAuthorities.isRootAuthority = true;
certificateAuthorities.certificate = "Binary";
certificateAuthoritiesList.add(certificateAuthorities);
certificateBasedAuthConfiguration.certificateAuthorities = certificateAuthoritiesList;

graphClient.organization("{id}").certificateBasedAuthConfiguration().references()
    .buildRequest()
    .post(certificateBasedAuthConfiguration);

```