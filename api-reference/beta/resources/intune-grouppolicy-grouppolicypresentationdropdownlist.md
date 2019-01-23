---
title: tipo de recurso de groupPolicyPresentationDropdownList
description: Representa um elemento de dropdownList ADMX e um elemento de enum ADMX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c7f35a52e43598f09b3fccdce1ef1d869798e7b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429194"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>tipo de recurso de groupPolicyPresentationDropdownList

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um elemento de dropdownList ADMX e um elemento de enum ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationDropdownLists](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|coleção [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Obter groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Criar groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Crie um novo objeto de [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|
|[Excluir groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|Nenhum|Exclui um [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).|
|[Atualizar groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|Atualize as propriedades de um objeto [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|Valor de cadeia de caracteres localizada que identifica a opção padrão da lista de itens.|
|items|coleção [groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|Representa um conjunto de nomes de exibição localizado e seus valores associados.|
|obrigatório|Boolean|Requisito para inserir um valor na caixa de parâmetro. O valor padrão é false.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "String",
    "value": "String"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "String",
      "value": "String"
    }
  ],
  "required": true
}
```




