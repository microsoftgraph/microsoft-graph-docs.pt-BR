---
title: tipo de recurso securityBaselineTemplate
description: O modelo de linha de base de segurança da conta
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a464b12eca422241421137b0041660922ee8040
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943463"
---
# <a name="securitybaselinetemplate-resource-type"></a>tipo de recurso securityBaselineTemplate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O modelo de linha de base de segurança da conta


Herda de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|coleção [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Listar Propriedades e relações dos objetos [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Obter securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Leia as propriedades e as relações do objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Criar securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Criar um novo objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .|
|[Excluir securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|Nenhum|Exclui [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md).|
|[Atualizar securityBaselineTemplate](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|Atualiza as propriedades de um objeto [securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo herdada de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|String|O nome de exibição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|A descrição do modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|Cadeia de caracteres|As informações de versão do modelo herdadas de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|preterido|Booliano|O modelo é preterido ou não. Os propósitos não podem ser criados a partir de um modelo preterido. Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|intentCount|Int32|Número de tentativas criadas a partir deste modelo. Herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settings|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações que este modelo herdou de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|categories|coleção [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Conjunto de categorias de configuração no modelo herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|migratableTo|coleção [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Coleção de modelos que esse modelo pode migrar para herdado de [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|O resumo do estado do dispositivo de linha de base de segurança|
|deviceStates|coleção [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)|O dispositivo de linha de base de segurança indica|
|categoryDeviceStateSummaries|coleção [securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|O resumo do estado do dispositivo de linha de base de segurança por categoria|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024
}
```




