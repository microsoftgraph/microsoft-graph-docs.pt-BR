---
title: Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference
description: Definindo informações de referência do modelo de valor
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e08b43175b1f685a8883f63769bd91e974744f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091500"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo informações de referência do modelo de valor

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingValueTemplateId|Cadeia de Caracteres|Definindo a id do modelo de valor|
|useTemplateDefault|Boleano|Indica se o valor de configuração da política deve ser atualizado para corresponder ao valor padrão da configuração do modelo|

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



