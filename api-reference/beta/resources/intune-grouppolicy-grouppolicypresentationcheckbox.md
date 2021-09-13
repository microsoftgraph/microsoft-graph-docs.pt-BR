---
title: Tipo de recurso groupPolicyPresentationCheckBox
description: Representa um elemento checkBox ADMX e um elemento booleano ADMX.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9afa92ae390e26f3198c48df9b60e09facbbf10
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086089"
---
# <a name="grouppolicypresentationcheckbox-resource-type"></a>Tipo de recurso groupPolicyPresentationCheckBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento checkBox ADMX e um elemento booleano ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationCheckBoxes](../api/intune-grouppolicy-grouppolicypresentationcheckbox-list.md)|[coleção groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Obter groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-get.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Leia propriedades e relações do [objeto groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Criar groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-create.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Crie um novo [objeto groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|
|[Excluir groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md).|
|[Atualizar groupPolicyPresentationCheckBox](../api/intune-grouppolicy-grouppolicypresentationcheckbox-update.md)|[groupPolicyPresentationCheckBox](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationCheckBox.](../resources/intune-grouppolicy-grouppolicypresentationcheckbox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de Caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultChecked|Boleano|Valor padrão da caixa de seleção. O valor padrão é falso.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



