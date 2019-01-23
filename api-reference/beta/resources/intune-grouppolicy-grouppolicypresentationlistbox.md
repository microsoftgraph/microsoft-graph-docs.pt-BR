---
title: tipo de recurso de groupPolicyPresentationListBox
description: Representa um elemento de listBox ADMX e um elemento de lista ADMX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2cde4a73456975629af81de676e593c3fec3e211
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429213"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>tipo de recurso de groupPolicyPresentationListBox

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um elemento de listBox ADMX e um elemento de lista ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationListBoxes](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|coleção [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Obter groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Criar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Crie um novo objeto de [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|
|[Excluir groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Nenhum|Exclui um [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[Atualizar groupPolicyPresentationListBox](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Atualize as propriedades de um objeto [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Boolean|Se essa opção é especificada true o usuário deve especificar o valor da subchave do registro e o nome da subchave do registro. Caixa de listagem mostra duas colunas, um para o nome e outro para os dados. O valor padrão é false.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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
  "explicitValue": true
}
```




