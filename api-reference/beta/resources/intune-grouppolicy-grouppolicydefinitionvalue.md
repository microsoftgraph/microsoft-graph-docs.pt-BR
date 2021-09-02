---
title: Tipo de recurso groupPolicyDefinitionValue
description: A entidade de valor de definição armazena o valor para uma definição de política de grupo único.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f448796d720369185fee2a2fe1bc3c19256eb73
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796492"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>Tipo de recurso groupPolicyDefinitionValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de valor de definição armazena o valor para uma definição de política de grupo único.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyDefinitionValues](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|[coleção groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Listar propriedades e relações dos [objetos groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Obter groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Ler propriedades e relações do [objeto groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Criar groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Crie um novo [objeto groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|
|[Excluir groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|Nenhum(a)|Exclui um [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).|
|[Atualizar groupPolicyDefinitionValue](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Atualize as propriedades de [um objeto groupPolicyDefinitionValue.](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado.|
|enabled|Boolean|Habilita ou desabilita a definição de política de grupo associada.|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|Especifica como o valor deve ser configurado. Isso pode ser como uma Política ou como Uma Preferência. Os valores possíveis são: `policy` e `preference`.|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|presentationValues|[coleção groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Os valores de apresentação de política de grupo associados com o valor de definição.|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada ao valor.|

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



