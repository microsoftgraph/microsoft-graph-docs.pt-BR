---
title: tipo de recurso de groupPolicyPresentationComboBox
description: Representa um elemento de comboBox ADMX e um elemento de texto ADMX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2225cda293bd2966dd39347dfe1ed03b2a4137c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431257"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>tipo de recurso de groupPolicyPresentationComboBox

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um elemento de comboBox ADMX e um elemento de texto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationComboBoxes](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|coleção [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Obter groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Criar groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Crie um novo objeto de [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|
|[Excluir groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).|
|[Atualizar groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Atualize as propriedades de um objeto [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|String|Cadeia de caracteres localizadas padrão exibida na caixa de combinação. O valor padrão é vazio.|
|sugestões|String collection|Cadeias de caracteres localizadas listadas na lista suspensa da caixa de combinação. O valor padrão é vazio.|
|obrigatório|Boolean|Especifica se deve ser especificado um valor para o parâmetro. O valor padrão é false.|
|maxLength|Int64|Um inteiro não assinado que especifica o número máximo de caracteres de texto para o parâmetro. O valor padrão é 1023.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationComboBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "suggestions": [
    "String"
  ],
  "required": true,
  "maxLength": 1024
}
```




