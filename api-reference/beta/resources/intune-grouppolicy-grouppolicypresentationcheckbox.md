---
title: tipo de recurso de groupPolicyPresentationCheckBox
description: Representa um elemento de caixa de seleção ADMX e um elemento de booleano ADMX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b1427f3a2466d996e067b464a9d15a3db086314b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429225"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>tipo de recurso de groupPolicyPresentationCheckBox

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um elemento de caixa de seleção ADMX e um elemento de booleano ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationCheckBoxes](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|coleção [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Obter groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Criar groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Crie um novo objeto de [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|
|[Excluir groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).|
|[Atualizar groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Atualize as propriedades de um objeto [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultChecked|Boolean|Valor padrão para a caixa de seleção. O valor padrão é false.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationCheckBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationCheckBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultChecked": true
}
```




