---
title: Tipo de recurso groupPolicyConfiguration
description: A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46f23dc14427b9f4c7feb55f9538b010574b508
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063892"
---
# <a name="grouppolicyconfiguration-resource-type"></a>Tipo de recurso groupPolicyConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de configuração de política de grupo contém os valores configurados para uma ou mais definições de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[coleção groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Listar propriedades e relações dos [objetos groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Obter groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Leia propriedades e relações do [objeto groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Criar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Crie um novo [objeto groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Excluir groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Nenhum|Exclui um [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[Atualizar groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Atualize as propriedades de [um objeto groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[atribuir ação](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[coleção groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Ainda não documentado|
|[Ação updateDefinitionValues](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado.|
|displayName|String|Nome fornecido pelo usuário para o objeto resource.|
|description|Cadeia de caracteres|O usuário forneceu a descrição do objeto resource.|
|roleScopeTagIds|String collection|A lista de marcas de escopo para a configuração.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValues|[coleção groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|A lista de valores de definição de política de grupo habilitados ou desabilitados para a configuração.|
|assignments|[coleção groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|A lista de atribuições de grupo para a configuração.|

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
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



