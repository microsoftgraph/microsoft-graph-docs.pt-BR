---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 1e0efd19d7ffec7e8f710187830582a6239402d2
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2021
ms.locfileid: "53578932"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-reporting-service-limits"></a>Limites do serviço para relatórios do Intune

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
applicationSignInDetailedSummary, applicationSignInSummary, auditLogRoot, authenticationMethodsRoot, azureADFeatureUsage, azureADLicenseUsage, azureADUserFeatureUsage, credentialUsageSummary, credentialUserRegistrationCount, credentialUserRegistrationDetails, directoryAudit, provisioningObjectSummary, recommendation, recommendationResource, relyingPartyDetailedSummary, restrictedSignIn, signIn, userCredentialUsageDetails.
