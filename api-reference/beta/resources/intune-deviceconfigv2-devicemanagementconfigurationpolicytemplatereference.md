---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplateReference
description: Informações de referência do modelo de política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64bb59f9d96386260267890dbdce77c538afedcd
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60488350"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationPolicyTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de referência do modelo de política

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|templateId|Cadeia de caracteres|ID do modelo|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|Família de modelos do Modelo referenciado. Essa propriedade é somente leitura. Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`, `baseline`.|
|templateDisplayName|Cadeia de caracteres|Template Display Name of the referenced template. Essa propriedade é somente leitura.|
|templateDisplayVersion|Cadeia de caracteres|Template Display Version of the referenced Template. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyTemplateReference",
  "templateId": "String",
  "templateFamily": "String",
  "templateDisplayName": "String",
  "templateDisplayVersion": "String"
}
```



