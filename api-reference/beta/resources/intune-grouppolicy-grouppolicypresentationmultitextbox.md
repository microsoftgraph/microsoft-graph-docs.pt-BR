---
title: tipo de recurso groupPolicyPresentationMultiTextBox
description: Representa um elemento multiTextBox de ADMX e um elemento de multiTexto ADMX.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f17177b55d6033b35c4476e9df61150e785ba45
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784457"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>tipo de recurso groupPolicyPresentationMultiTextBox

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento multiTextBox de ADMX e um elemento de multiTexto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationMultiTextBoxes](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|coleção [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Obter groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Criar groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Criar um novo objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|
|[Excluir groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|Nenhum|Exclui [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[Atualizar groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|obrigatório|Booliano|Requisito para inserir um valor na caixa de texto. O valor padrão é falso.|
|maxLength|Int64|Um inteiro sem sinal que especifica o número máximo de caracteres de texto. O valor padrão é 1023.|
|maxStrings|Int64|Um inteiro sem sinal que especifica o número máximo de cadeias de caracteres. O valor padrão é 0.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definir|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```





