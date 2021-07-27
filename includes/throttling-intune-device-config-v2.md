---
author: davidmu1
localization_priority: Priority
ms.prod: msgraph
ms.topic: include
ms.openlocfilehash: a34d9ff1133dc9f996ea1afe10b49a19faa00658
ms.sourcegitcommit: 10d9f4c2cee192bd80984d48cabba63b47c54551
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2021
ms.locfileid: "53578918"
---
<!-- markdownlint-disable MD041 -->
<!-- this file is auto-generated don't edit it manually! -->
#### <a name="intune-device-config-v2-service-limits"></a>Limites de serviço V2 de configuração de dispositivo do Intune

| Tipo de solicitação | Limitar por locatário para todos os aplicativos | Limitar por aplicativo por locatário |
| ------------ | ----------------------------- | ------------------------ |
| POST, PUT, DELATE, PATCH | 200 solicitações por 20 segundos | 100 solicitações por 20 segundos |
| Qualquer | 2000 solicitações por 20 segundos | 1000 solicitações por 20 segundos |

Os limites anteriores se aplicam aos seguintes recursos:  
deviceManagementConfigurationCategory, deviceManagementConfigurationChoiceSettingCollectionDefinition, deviceManagementConfigurationChoiceSettingDefinition, deviceManagementConfigurationPolicy, deviceManagementConfigurationPolicyAssignment, deviceManagementConfigurationPolicyTemplate, deviceManagementConfigurationSetting, deviceManagementConfigurationSettingDefinition, deviceManagementConfigurationSettingGroupCollectionDefinition, deviceManagementConfigurationSettingGroupDefinition, deviceManagementConfigurationSettingTemplate, deviceManagementConfigurationSimpleSettingCollectionDefinition, deviceManagementConfigurationSimpleSettingDefinition, deviceManagementReusablePolicySetting.
