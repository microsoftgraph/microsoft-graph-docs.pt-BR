---
title: Tipo de recurso groupPolicyPresentationValueLongDecimal
description: A entidade representa um valor longo não assinado de uma apresentação de caixa de texto decimal longa em uma definição de política.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 506bb379a85ed12b2b59f41113fee47359c0d9fb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818769"
---
# <a name="grouppolicypresentationvaluelongdecimal-resource-type"></a>Tipo de recurso groupPolicyPresentationValueLongDecimal

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um valor longo não assinado de uma apresentação de caixa de texto decimal longa em uma definição de política.


Herda de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValueLongDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-list.md)|[coleção groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Obter groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-get.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Leia propriedades e relações do [objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Criar groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-create.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Crie um novo [objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|
|[Excluir groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md).|
|[Atualizar groupPolicyPresentationValueLongDecimal](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-update.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValueLongDecimal.](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|valor|Int64|Um valor longo não assinado para a apresentação associada.|

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



