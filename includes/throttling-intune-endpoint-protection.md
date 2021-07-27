---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: d6c48f17f0d54a475632d37bbfcc500f6c788742
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2021
ms.locfileid: "53578923"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-endpoint-protection-service-limits"></a>Limites de serviço do Intune Endpoint Protection

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
deviceManagementDerivedCredentialSettings, deviceManagementResourceAccessProfileAssignment, deviceManagementResourceAccessProfileBase, windows10XCertificateProfile, windows10XSCEPCertificateProfile, windows10XTrustedRootCertificate, windows10XVpnConfiguration, windows10XWifiConfiguration.
