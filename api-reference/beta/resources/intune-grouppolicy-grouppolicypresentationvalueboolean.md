---
title: tipo de recurso groupPolicyPresentationValueBoolean
description: A entidade representa um valor Boolean de uma apresentação de caixa de seleção em uma definição de política.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 98003da9fee60e538c18d9267eda677790a2ce23
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068932"
---
# <a name="grouppolicypresentationvalueboolean-resource-type"></a>tipo de recurso groupPolicyPresentationValueBoolean

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor Boolean de uma apresentação de caixa de seleção em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueBooleans](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-list.md)|[coleção groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Obter groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Ler propriedades e relações do [objeto groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Criar groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Crie um novo [objeto groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|
|[Excluir groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md).|
|[Atualizar groupPolicyPresentationValueBoolean](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValueBoolean.](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|Boolean|Um valor booleano para a apresentação associada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição de política de grupo associado ao valor de apresentação. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|presentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação da política de grupo associada ao valor de apresentação. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": true
}
```



