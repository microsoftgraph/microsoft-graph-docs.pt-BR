---
title: Tipo de recurso groupPolicyPresentationValueDecimal
description: A entidade representa um valor inteiro não assinado de uma apresentação de caixa de texto decimal em uma definição de política.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: feeb282e3d776eebc9959a0277d3a2bc8bd39135
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068897"
---
# <a name="grouppolicypresentationvaluedecimal-resource-type"></a>Tipo de recurso groupPolicyPresentationValueDecimal

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor inteiro não assinado de uma apresentação de caixa de texto decimal em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-list.md)|[coleção groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValueDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|
|[Obter groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-get.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|Leia propriedades e relações do [objeto groupPolicyPresentationValueDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|
|[Criar groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-create.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|Crie um novo [objeto groupPolicyPresentationValueDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|
|[Excluir groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md).|
|[Atualizar groupPolicyPresentationValueDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluedecimal-update.md)|[groupPolicyPresentationValueDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValueDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluedecimal.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|valor|Int64|Um valor inteiro não assinado para a apresentação associada.|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueDecimal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueDecimal",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": 1024
}
```



