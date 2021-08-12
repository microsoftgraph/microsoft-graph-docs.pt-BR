---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: e1abf2e2dc61b5a9bb601ee31af7bd2f6defacd2b748066111623bd2647e3a9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196592"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-enrollment-service-limits"></a>Limites do serviço para inscrição do Intune

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
complianceManagementPartner, deviceAppManagement, deviceCategory, deviceComanagementAuthorityConfiguration, deviceEnrollmentConfiguration, deviceEnrollmentLimitConfiguration, deviceEnrollmentPlatformRestrictionsConfiguration, deviceEnrollmentWindowsHelloForBusinessConfiguration, deviceManagementExchangeConnector, deviceManagementExchangeOnPremisesPolicy, deviceManagementPartner, enrollmentConfigurationAssignment, mobileThreatDefenseConnector, onPremisesConditionalAccessSettings, sideLoadingKey, vppToken, windows10EnrollmentCompletionPageConfiguration.
