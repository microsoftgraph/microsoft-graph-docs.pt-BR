---
title: Tipo de recurso groupPolicyPresentationValueText
description: A entidade representa um valor de cadeia de caracteres para uma lista lista, caixa de combinação ou apresentação de caixa de texto em uma definição de política.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75927a6c8e0063a6d306750a7095f10a8ce5de56
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821105"
---
# <a name="grouppolicypresentationvaluetext-resource-type"></a>Tipo de recurso groupPolicyPresentationValueText

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor de cadeia de caracteres para uma lista lista, caixa de combinação ou apresentação de caixa de texto em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueTexts](../api/intune-grouppolicy-grouppolicypresentationvaluetext-list.md)|[coleção groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|
|[Obter groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-get.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Leia propriedades e relações do [objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|
|[Criar groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-create.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Crie um novo [objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|
|[Excluir groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).|
|[Atualizar groupPolicyPresentationValueText](../api/intune-grouppolicy-grouppolicypresentationvaluetext-update.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValueText.](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Chave da entidade. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|value|Cadeia de caracteres|Um valor de cadeia de caracteres para a apresentação associada.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": "String"
}
```



