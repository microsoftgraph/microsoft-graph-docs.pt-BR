---
title: Tipo de recurso groupPolicyPresentationComboBox
description: Representa um elemento comboBox ADMX e um elemento de texto ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a83f1bb87a13c9dd49ff352f82bc87f5301967f987f5eeff2748d8e1b0a0d662
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54214954"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>Tipo de recurso groupPolicyPresentationComboBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento comboBox ADMX e um elemento de texto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationComboBoxes](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[coleção groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Obter groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Leia propriedades e relações do [objeto groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Criar groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Crie um novo [objeto groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|
|[Excluir groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).|
|[Atualizar groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationComboBox.](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Cadeia de caracteres|Cadeia de caracteres padrão localizada exibida na caixa de combinação. O valor padrão é vazio.|
|sugestões|String collection|Cadeias de caracteres localizadas listadas na listada da caixa de combinação. O valor padrão é vazio.|
|obrigatório|Boolean|Especifica se um valor deve ser especificado para o parâmetro. O valor padrão é falso.|
|maxLength|Int64|Um inteiro não assinado que especifica o número máximo de caracteres de texto para o parâmetro. O valor padrão é 1023.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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




