---
title: tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos gerenciados
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 42a92fd725c9f0b99037825c240dd017bf6c9c82
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060773"
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
|totalComanagedCount|Int32|Número de dispositivos co-gerenciados. Essa propriedade é somente leitura.|

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






