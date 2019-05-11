---
title: tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d910bf8bdef34c60ca6bb66e1ce87ca9cf1d51ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941174"
---
# <a name="grouppolicyconfiguration-resource-type"></a>tipo de recurso groupPolicyConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Listar Propriedades e relações dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Obter groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Leia as propriedades e as relações do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Criar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Criar um novo objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Excluir groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Nenhum|Exclui [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[Atualizar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Atualiza as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[atribuir ação](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado.|
|displayName|String|Nome fornecido pelo usuário para o objeto Resource.|
|description|String|Descrição fornecida pelo usuário para o objeto Resource.|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValues|coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.|
|assignments|coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|A lista de atribuições de grupo para a configuração.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




