---
title: tipo de recurso groupPolicyPresentationTextBox
description: Representa um elemento textBox do ADMX e um elemento de texto do ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f5b967e0366cdae2afd4fe28a7ee9bf7cbc7760
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941041"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>tipo de recurso groupPolicyPresentationTextBox

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento textBox do ADMX e um elemento de texto do ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationTextBoxes](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|coleção [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Obter groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Criar groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Criar um novo objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|
|[Excluir groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|Nenhum|Exclui [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).|
|[Atualizar groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Cadeia de caracteres|Cadeia de caracteres padrão localizada exibida na caixa de texto. O valor padrão é vazio.|
|obrigatório|Booliano|Requisito para inserir um valor na caixa de texto. O valor padrão é falso.|
|maxLength|Int64|Um inteiro sem sinal que especifica o número máximo de caracteres de texto. O valor padrão é 1023.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definir|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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




