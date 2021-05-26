---
title: Tipo de recurso deviceManagementConfigurationPolicyTemplateReference
description: Informações de referência do modelo de política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff61ac1e881ec6bb40750d9cb43d80c6722dd79e
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666496"
---
# <a name="devicemanagementconfigurationpolicytemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationPolicyTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de referência do modelo de política

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|templateId|String|ID do modelo|
|templateFamily|[deviceManagementConfigurationTemplateFamily](../resources/intune-deviceconfigv2-devicemanagementconfigurationtemplatefamily.md)|Família de modelos do Modelo referenciado. Essa propriedade é somente leitura. Os valores possíveis são: `none`, `endpointSecurityAntivirus`, `endpointSecurityDiskEncryption`, `endpointSecurityFirewall`, `endpointSecurityEndpointDetectionAndResponse`, `endpointSecurityAttackSurfaceReduction`, `endpointSecurityAccountProtection`, `endpointSecurityApplicationControl`.|
|templateDisplayName|String|Template Display Name of the referenced template. Essa propriedade é somente leitura.|
|templateDisplayVersion|String|Template Display Version of the referenced Template. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
Nenhuma

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




