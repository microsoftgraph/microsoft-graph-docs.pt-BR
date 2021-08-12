---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 17b5355ba3a51308822c5870d5ca0beafd5bf4ae69abc7914768f0cd1757b9c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196602"
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
