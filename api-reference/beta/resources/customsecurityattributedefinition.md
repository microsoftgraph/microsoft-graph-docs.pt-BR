---
title: Tipo de recurso customSecurityAttributeDefinition
description: Um objeto que representa o esquema de um atributo de segurança personalizado (par de valores-chave).
author: rolyon
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 390af00d09d2b54fde5bf1cf510ad1752038d3fa
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077674"
---
# <a name="customsecurityattributedefinition-resource-type"></a>Tipo de recurso customSecurityAttributeDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto que representa o esquema de um atributo de segurança personalizado (par de valores-chave). Por exemplo, o nome do atributo de segurança personalizado, a descrição, o tipo de dados e os valores permitidos.

Até 500 objetos ativos podem ser definidos em um locatário. O objeto não pode ser renomeado ou excluído, mas pode ser desativado usando a `customSecurityAttributeDefiniton` [operação Update customSecurityAttributeDefinition.](../api/customsecurityattributedefinition-update.md) Deve fazer parte de um conjunto de atributos.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar customSecurityAttributeDefinitions](../api/directory-list-customsecurityattributedefinitions.md)|[Coleção customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Obter uma lista dos [objetos customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) e suas propriedades.|
|[Obter customSecurityAttributeDefinition](../api/customsecurityattributedefinition-get.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Leia as propriedades e as relações de um [objeto customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|
|[Criar customSecurityAttributeDefinition](../api/directory-post-customsecurityattributedefinitions.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Crie um novo [objeto customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|
|[Atualizar customSecurityAttributeDefinition](../api/customsecurityattributedefinition-update.md)|[customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md)|Atualize as propriedades de [um objeto customSecurityAttributeDefinition.](../resources/customsecurityattributedefinition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|attributeSet|Cadeia de caracteres|Nome do conjunto de atributos. Maiúsculas de minúsculas.|
|description|Cadeia de caracteres|Descrição do atributo de segurança personalizado. Pode ter até 128 caracteres e incluir caracteres Unicode. Pode ser alterado posteriormente.|
|id|String|Identificador do atributo de segurança personalizado, que é uma combinação do nome do conjunto de atributos e o nome do atributo de segurança personalizado separado por um sublinhado ( `attributeSet` _ `name` ). A `id` propriedade é gerada automaticamente e não pode ser definida. Maiúsculas de minúsculas.|
|isCollection|Boolean|Indica se vários valores podem ser atribuídos ao atributo de segurança personalizado. Não é possível alterá-los posteriormente. Se `type` estiver definido como Boolean, não será possível definir como `isCollection` true.|
|isSearchable|Booliano|Indica se os valores de atributo de segurança personalizados serão indexados para pesquisa em objetos atribuídos a valores de atributo. Não é possível alterá-los posteriormente.|
|nome|Cadeia de caracteres|Nome do atributo de segurança personalizado. Deve ser exclusivo em um conjunto de atributos. Pode ter até 32 caracteres e incluir caracteres Unicode. Não é possível conter espaços ou caracteres especiais. Não é possível alterá-los posteriormente. Maiúsculas de minúsculas.|
|status|String|Especifica se o atributo de segurança personalizado está ativo ou desativado. Os valores aceitáveis são `Available` e `Deprecated` . Pode ser alterado posteriormente.|
|type|Cadeia de caracteres|Tipo de dados para os valores de atributo de segurança personalizados. Os tipos com suporte `Boolean` são `Integer` , e `String` . Não é possível alterá-los posteriormente.|
|usePreDefinedValuesOnly|Booliano|Indica se somente valores predefinidos podem ser atribuídos ao atributo de segurança personalizado. Se definido como false, os valores de formulário livre serão permitidos. Posteriormente, pode ser alterado de true para false, mas não pode ser alterado de falso para verdadeiro. Se `type` estiver definido como Boolean, não será possível definir como `usePreDefinedValuesOnly` true. |


## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|allowedValues|[Coleção allowedValue](../resources/allowedvalue.md)|Valores predefinidos para esse atributo de segurança personalizado.<br><br>Essa propriedade de navegação não é retornada por padrão e deve ser especificada em `$expand` uma consulta. Por exemplo, `/directory/customSecurityAttributeDefinitions?$expand=allowedValues`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customSecurityAttributeDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSecurityAttributeDefinition",
  "attributeSet": "String",
  "description": "String",
  "id": "String (identifier)",
  "isCollection": "Boolean",
  "isSearchable": "Boolean",
  "name": "String",
  "status": "String",
  "type": "String",
  "usePreDefinedValuesOnly": "Boolean"
}
```
