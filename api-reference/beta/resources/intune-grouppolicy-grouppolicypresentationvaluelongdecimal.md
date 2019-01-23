---
title: tipo de recurso de groupPolicyPresentationValueLongDecimal
description: A entidade representa um valor longo não assinado de uma apresentação da caixa de texto longos decimal em uma definição de política.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ecdd82f6c0ca3481cd146d1a191565d7bc3250e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429263"
---
# <a name="grouppolicypresentationvaluelongdecimal-resource-type"></a>tipo de recurso de groupPolicyPresentationValueLongDecimal

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade representa um valor longo não assinado de uma apresentação da caixa de texto longos decimal em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationValueLongDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-list.md)|coleção [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .|
|[Obter groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-get.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .|
|[Criar groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-create.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Crie um novo objeto de [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .|
|[Excluir groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).|
|[Atualizar groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-update.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Atualize as propriedades de um objeto [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e hora que da última modificação do objeto. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e hora que o objeto foi criado. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|valor|Int64|Um valor long não assinado para a apresentação associado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição de política do grupo associado com o valor de apresentação. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|apresentação|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação de diretiva de grupo associada com o valor de apresentação. Herdado de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueLongDecimal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": 1024
}
```




