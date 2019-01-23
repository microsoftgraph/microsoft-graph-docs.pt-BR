---
title: tipo de recurso de groupPolicyConfiguration
description: A entidade de configuração de diretiva de grupo contém os valores configurados para uma ou mais definições de política de grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431305"
---
# <a name="grouppolicyconfiguration-resource-type"></a>tipo de recurso de groupPolicyConfiguration

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade de configuração de diretiva de grupo contém os valores configurados para uma ou mais definições de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|coleção [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Obter groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Criar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Crie um novo objeto de [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Excluir groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Nenhum|Exclui um [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[Atualizar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Atualize as propriedades de um objeto [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) .|
|[Ação assign](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|coleção [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e hora que o objeto foi criado.|
|displayName|String|Nome de usuário fornecido para o objeto resource.|
|description|String|Descrição para o objeto resource fornecidos pelo usuário.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValues|coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|A lista de habilitada ou desabilitada valores de definição de diretiva de grupo para a configuração.|
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




