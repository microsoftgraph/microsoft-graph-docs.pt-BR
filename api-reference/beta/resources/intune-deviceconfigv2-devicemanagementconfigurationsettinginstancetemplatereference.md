---
title: Tipo de recurso deviceManagementConfigurationSettingInstanceTemplateReference
description: Definindo informações de referência do modelo de instância
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c4990ef6219ba6f15a3af5eb76a290cc007b7b43
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59148400"
---
# <a name="devicemanagementconfigurationsettinginstancetemplatereference-resource-type"></a>Tipo de recurso deviceManagementConfigurationSettingInstanceTemplateReference

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Definindo informações de referência do modelo de instância

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|settingInstanceTemplateId|Cadeia de Caracteres|ID do modelo de instância de configuração|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
  "settingInstanceTemplateId": "String"
}
```



