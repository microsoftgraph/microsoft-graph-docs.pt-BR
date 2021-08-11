---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: cafb23b7b427b75bf0b8f357947c2c5275bb074755f1c0353b1a86cfecaa099c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196598"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-partner-integration-service-limits"></a>Limites do serviço de integração de parceiros do Intune

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
appVulnerabilityManagedDevice, appVulnerabilityMobileApp, appVulnerabilityTask, configManagerCollection, deviceAppManagementTask, securityConfigurationTask, unmanagedDeviceDiscoveryTask, vulnerableManagedDevice.
