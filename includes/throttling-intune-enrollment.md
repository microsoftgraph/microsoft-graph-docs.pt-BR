---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: 656be4e351881a16f7b517902e7576d23dae9b7b
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2021
ms.locfileid: "53578922"
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
