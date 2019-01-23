---
title: tipo de recurso de groupPolicyDefinitionValue
description: A entidade de valor de definição armazena o valor de uma definição de política de grupo único.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7e98a41409efba60ee1431fac82a49be2029039
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429214"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>tipo de recurso de groupPolicyDefinitionValue

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade de valor de definição armazena o valor de uma definição de política de grupo único.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyDefinitionValues](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|coleção [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Obter groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Criar groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Crie um novo objeto de [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|
|[Excluir groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|Nenhum|Exclui um [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).|
|[Atualizar groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Atualize as propriedades de um objeto [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e hora que o objeto foi criado.|
|enabled|Boolean|Habilita ou desabilita a definição de política de grupo associado.|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|Especifica como o valor deve ser configurado. Isso pode ser como uma política ou como uma preferência. Os valores possíveis são: `policy` e `preference`.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|presentationValues|coleção [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Os valores de apresentação de diretiva de grupo associado com o valor de definição.|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associado com o valor.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




