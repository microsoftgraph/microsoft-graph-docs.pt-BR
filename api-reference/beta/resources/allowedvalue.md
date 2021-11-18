---
title: Tipo de recurso allowedValue
description: Um valor predefinido que é permitido para uma definição de atributo de segurança personalizada.
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 21e6b1836ae23e1cc6b7c78053ff458ac934087e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077469"
---
# <a name="allowedvalue-resource-type"></a>Tipo de recurso allowedValue

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um valor predefinido que é permitido para uma definição de atributo de segurança personalizada.

Até 100 `allowedValue` objetos podem ser definidos por [customSecurityAttributeDefinition](customsecurityattributedefinition.md). Esse objeto não pode ser renomeado ou excluído, mas pode ser desativado usando a [operação Update allowedValue.](../api/../api/allowedvalue-update.md) Esse objeto é definido como uma propriedade de navegação no [recurso customSecurityAttributeDefinition](customsecurityattributedefinition.md) e seu valor é retornado somente em `$expand` .

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar allowedValues](../api/customsecurityattributedefinition-list-allowedvalues.md)|[Coleção allowedValue](../resources/allowedvalue.md)|Obter uma lista dos [objetos allowedValue](../resources/allowedvalue.md) e suas propriedades.|
|[Obter allowedValue](../api/allowedvalue-get.md)|[allowedValue](../resources/allowedvalue.md)|Leia as propriedades e as relações de um [objeto allowedValue.](../resources/allowedvalue.md)|
|[Criar allowedValue](../api/customsecurityattributedefinition-post-allowedvalues.md)|[allowedValue](../resources/allowedvalue.md)|Crie um novo [objeto allowedValue.](../resources/allowedvalue.md)|
|[Atualizar allowedValue](../api/allowedvalue-update.md)|[allowedValue](../resources/allowedvalue.md)|Atualize as propriedades de um [objeto allowedValue.](../resources/allowedvalue.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| id | Cadeia de caracteres | Identificador do valor predefinido. Pode ter até 64 caracteres e incluir caracteres Unicode. Pode incluir espaços, mas alguns caracteres especiais não são permitidos. Não é possível alterá-los posteriormente. Case sensitive. |
|isActive|Boolean|Indica se o valor predefinido está ativo ou desativado. Se definido como , esse valor predefinido não poderá ser atribuído a `false` nenhum objeto de diretório com suporte adicional.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.allowedValue",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allowedValue",
  "id": "String (identifier)",
  "isActive": "Boolean"
}
```
