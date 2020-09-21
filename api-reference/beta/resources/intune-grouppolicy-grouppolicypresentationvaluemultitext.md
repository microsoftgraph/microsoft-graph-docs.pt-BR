---
title: tipo de recurso groupPolicyPresentationValueMultiText
description: A entidade representa um valor de cadeia de caracteres de uma apresentação de caixa de texto com várias linhas em uma definição de política.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a616d85703a5ccf890a0f314eaefe6f3ec57709
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030700"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>tipo de recurso groupPolicyPresentationValueMultiText

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor de cadeia de caracteres de uma apresentação de caixa de texto com várias linhas em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueMultiTexts](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|coleção [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Obter groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Criar groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Criar um novo objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|
|[Excluir groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|Nenhum|Exclui [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).|
|[Atualizar groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Coleção String|Uma coleção de cadeias de caracteres não vazias para a apresentação associada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionvalue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição da política de grupo associado ao valor da apresentação. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|apresentação|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação da política de grupo associada ao valor da apresentação. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    "String"
  ]
}
```






