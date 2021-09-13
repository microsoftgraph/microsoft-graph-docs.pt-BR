---
title: Tipo de recurso groupPolicyPresentationValueMultiText
description: A entidade representa um valor de cadeia de caracteres de uma apresentação de caixa de texto de várias linhas em uma definição de política.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31977668f31e1928750d4d75274f20b4741689ed
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033493"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>Tipo de recurso groupPolicyPresentationValueMultiText

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor de cadeia de caracteres de uma apresentação de caixa de texto de várias linhas em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueMultiTexts](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|[coleção groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Obter groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Ler propriedades e relações do [objeto groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Criar groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Crie um novo [objeto groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|
|[Excluir groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md).|
|[Atualizar groupPolicyPresentationValueMultiText](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValueMultiText.](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|values|Conjunto de cadeias de caracteres|Uma coleção de cadeias de caracteres não vazias para a apresentação associada.|

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



