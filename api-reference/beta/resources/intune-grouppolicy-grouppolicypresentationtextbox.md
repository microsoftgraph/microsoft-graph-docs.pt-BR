---
title: Tipo de recurso groupPolicyPresentationTextBox
description: Representa um elemento textBox ADMX e um elemento de texto ADMX.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 01ba00d4cff15e73917d88e01769e228a1320100
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085970"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>Tipo de recurso groupPolicyPresentationTextBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento textBox ADMX e um elemento de texto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationTextBoxes](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|[coleção groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Listar propriedades e relações dos objetos [groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|
|[Obter groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Leia propriedades e relações do [objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|
|[Criar groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Crie um novo [objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|
|[Excluir groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).|
|[Atualizar groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationTextBox.](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de Caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Cadeia de Caracteres|Cadeia de caracteres padrão localizada exibida na caixa de texto. O valor padrão é vazio.|
|obrigatório|Boleano|Requisito para inserir um valor na caixa de texto. O valor padrão é falso.|
|maxLength|Int64|Um inteiro não assinado que especifica o número máximo de caracteres de texto. O valor padrão é 1023.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "required": true,
  "maxLength": 1024
}
```



