---
title: Tipo de recurso groupPolicyPresentationMultiTextBox
description: Representa um elemento ADMX multiTextBox e um elemento ADMX multiText.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 957cd32c2ebdbb808ba90e31a9d013957f1366c6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039781"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>Tipo de recurso groupPolicyPresentationMultiTextBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento ADMX multiTextBox e um elemento ADMX multiText.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationMultiTextBoxes](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|[coleção groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|
|[Obter groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Leia propriedades e relações do [objeto groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|
|[Criar groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Crie um novo [objeto groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|
|[Excluir groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[Atualizar groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationMultiTextBox.](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de Caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|obrigatório|Boleano|Requisito para inserir um valor na caixa de texto. O valor padrão é falso.|
|maxLength|Int64|Um inteiro não assinado que especifica o número máximo de caracteres de texto. O valor padrão é 1023.|
|maxStrings|Int64|Um inteiro não assinado que especifica o número máximo de cadeias de caracteres. O valor padrão é 0.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



