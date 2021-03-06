---
title: tipo de recurso groupPolicyPresentationValue
description: A entidade de valor de apresentação base que armazena o valor de uma única apresentação de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d44ce8e11ae1f44d10518ea2b1b0c990153923cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222804"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>tipo de recurso groupPolicyPresentationValue

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de valor de apresentação base que armazena o valor de uma única apresentação de política de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|coleção [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Obter groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Criar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Criar um novo objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Excluir groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Nenhum|Exclui [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Atualizar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez.|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado.|
|id|String|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionvalue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição da política de grupo associado ao valor da apresentação.|
|apresentação|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação da política de grupo associada ao valor da apresentação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




