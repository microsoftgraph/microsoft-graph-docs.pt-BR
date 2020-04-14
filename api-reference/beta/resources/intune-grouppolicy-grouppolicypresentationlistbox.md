---
title: tipo de recurso groupPolicyPresentationListBox
description: Representa um elemento listBox do ADMX e um elemento de lista ADMX.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1fb7a2e7cad8785b23eaf14e165d3d7b28b9beb2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462442"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>tipo de recurso groupPolicyPresentationListBox

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento listBox do ADMX e um elemento de lista ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationListBoxes](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|coleção [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Obter groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Criar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Criar um novo objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Excluir groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Nenhum|Exclui [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[Atualizar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Booliano|Se essa opção for especificada true, o usuário deverá especificar o valor da subchave do registro e o nome da subchave do registro. A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados. O valor padrão é falso.|
|valuePrefix|String|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definir|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true,
  "valuePrefix": "String"
}
```



