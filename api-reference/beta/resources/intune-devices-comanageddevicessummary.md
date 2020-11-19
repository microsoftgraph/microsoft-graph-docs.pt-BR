---
title: tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b25820e4356fadaa4f991c103500a8ef8f5c0122
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214845"
---
# <a name="comanageddevicessummary-resource-type"></a>tipo de recurso comanagedDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dados de resumo para dispositivos gerenciados

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inventoryCount|Int32|Número de dispositivos com Swung de inventário. Essa propriedade é somente leitura.|
|compliancePolicyCount|Int32|Número de dispositivos com o CompliancePolicy de Swung. Essa propriedade é somente leitura.|
|resourceAccessCount|Int32|Número de dispositivos com o ResourceAccess de Swung. Essa propriedade é somente leitura.|
|configurationSettingsCount|Int32|Número de dispositivos com o ConfigurationSettings de Swung. Essa propriedade é somente leitura.|
|windowsUpdateForBusinessCount|Int32|Número de dispositivos com o WindowsUpdateForBusiness de Swung. Essa propriedade é somente leitura.|
|endpointProtectionCount|Int32|Número de dispositivos com o EndpointProtection de Swung. Essa propriedade é somente leitura.|
|modernAppsCount|Int32|Número de dispositivos com o ModernApps de Swung. Essa propriedade é somente leitura.|
|officeAppsCount|Int32|Número de dispositivos com o Officetreinamento de Swung. Essa propriedade é somente leitura.|
|totalComanagedCount|Int32|Número de dispositivos de Co-Managed. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagedDevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.comanagedDevicesSummary",
  "inventoryCount": 1024,
  "compliancePolicyCount": 1024,
  "resourceAccessCount": 1024,
  "configurationSettingsCount": 1024,
  "windowsUpdateForBusinessCount": 1024,
  "endpointProtectionCount": 1024,
  "modernAppsCount": 1024,
  "officeAppsCount": 1024,
  "totalComanagedCount": 1024
}
```




