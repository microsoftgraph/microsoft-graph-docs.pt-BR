---
title: Tipo de recurso comanagedDevicesSummary
description: Dados de resumo para dispositivos co gerenciados
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa734753a13777e93f8018ce0e13267a485044a7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137851"
---
# <a name="comanageddevicessummary-resource-type"></a>Tipo de recurso comanagedDevicesSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dados de resumo para dispositivos co gerenciados

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inventoryCount|Int32|Número de dispositivos com o Inventário reatados. Essa propriedade é somente leitura.|
|compliancePolicyCount|Int32|Número de dispositivos com CompliancePolicy reatados. Essa propriedade é somente leitura.|
|resourceAccessCount|Int32|Número de dispositivos com ResourceAccess reatados. Essa propriedade é somente leitura.|
|configurationSettingsCount|Int32|Número de dispositivos com ConfigurationSettings reatados. Essa propriedade é somente leitura.|
|windowsUpdateForBusinessCount|Int32|Número de dispositivos com o WindowsUpdateForBusiness balanceado. Essa propriedade é somente leitura.|
|endpointProtectionCount|Int32|Número de dispositivos com EndpointProtection balanceado. Essa propriedade é somente leitura.|
|modernAppsCount|Int32|Número de dispositivos com ModernApps reatados. Essa propriedade é somente leitura.|
|officeAppsCount|Int32|Número de dispositivos com OfficeApps reatados. Essa propriedade é somente leitura.|
|totalComanagedCount|Int32|Número de Co-Managed Dispositivos. Essa propriedade é somente leitura.|

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



