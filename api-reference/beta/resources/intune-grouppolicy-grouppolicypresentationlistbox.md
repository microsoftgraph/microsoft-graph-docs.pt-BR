---
title: Tipo de recurso groupPolicyPresentationListBox
description: Representa um elemento listBox ADMX e um elemento de lista ADMX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9c5e121d08bb9cf362f75810dd014c5edb476af
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801462"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>Tipo de recurso groupPolicyPresentationListBox

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento listBox ADMX e um elemento de lista ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationListBoxes](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[coleção groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|
|[Obter groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Ler propriedades e relações do [objeto groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|
|[Criar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Crie um novo [objeto groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|
|[Excluir groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Nenhum(a)|Exclui um [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[Atualizar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Atualize as propriedades de [um objeto groupPolicyPresentationListBox.](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Boleano|Se essa opção for especificada como true, o usuário deverá especificar o valor da sub-chave do Registro e o nome da sub-chave do Registro. A caixa de listagem mostra duas colunas, uma para o nome e outra para os dados. O valor padrão é falso.|
|valuePrefix|String|Ainda não documentado|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



