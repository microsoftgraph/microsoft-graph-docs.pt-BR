---
title: Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference
description: Definindo informações de referência do modelo de valor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671543"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo informações de referência do modelo de valor

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateId|Cadeia de Caracteres|Definindo a ID do modelo de valor|
|useTemplateDefault|Boolean|Indica se o valor da configuração de política deve ser atualizado para corresponder ao valor padrão da configuração do modelo|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




