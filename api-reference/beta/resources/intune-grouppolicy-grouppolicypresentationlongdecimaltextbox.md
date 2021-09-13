---
title: Tipo de recurso groupPolicyPresentationLongDecimalTextBox
description: Representa um elemento ADMX longDecimalTextBox e um elemento ADMX longDecimal.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc493139866c77c55002c4dc92cbe0880e00aeeb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046810"
---
# <a name="grouppolicypresentationlongdecimaltextbox-resource-type"></a>Tipo de recurso groupPolicyPresentationLongDecimalTextBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento ADMX longDecimalTextBox e um elemento ADMX longDecimal.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationLongDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-list.md)|[coleção groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Obter groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-get.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Leia propriedades e relações do [objeto groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Criar groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-create.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Crie um novo [objeto groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|
|[Excluir groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).|
|[Atualizar groupPolicyPresentationLongDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-update.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationLongDecimalTextBox.](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de Caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Um inteiro não assinado que especifica o valor inicial da caixa de texto decimal. O valor padrão é 1.|
|spin|Boleano|Se for true, crie um controle de rotação; caso contrário, crie uma caixa de texto para entrada numérica. O valor padrão é true.|
|spinStep|Int64|Um inteiro não assinado que especifica o incremento de alteração para o controle de rotação. O valor padrão é 1.|
|obrigatório|Boleano|Requisito para inserir um valor na caixa de parâmetros. O valor padrão é falso.|
|minValue|Int64|Um long não assinado que especifica o valor mínimo permitido. O valor padrão é 0.|
|maxValue|Int64|Um long não assinado que especifica o valor máximo permitido. O valor padrão é 9999.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationLongDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```



