---
title: tipo de recurso itens
description: Um objeto de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 438fa0035b2c84b6fe702e3b1765e3d8b5adaf9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006623"
---
# <a name="items-resource-type"></a>tipo de recurso itens
Representa um item no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                      |Tipo de retorno|Descrição |
|:--------------------------------------------|:----------|:-----------|
|[Obter itens](../api/dynamics-item-get.md)      |items     |Obtém um objeto item.   |
|[Itens post](../api/dynamics-create-item.md)  |items     |Cria um objeto item.|
|[Item de patch](../api/dynamics-item-update.md)  |items     |Atualiza um objeto item.|
|[Excluir itens](../api/dynamics-item-delete.md)|none      |Exclui um objeto item.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo |Descrição                                          |
|:-------------------|:-------|:----------------------------------------------------|
|id                  |GUID    |A ID exclusiva do item. Não editável.             |
|number              |string  |O número do item.                                     |
|displayName         |string  |Especifica uma descrição do item.                 |
|type                |numéricos |O tipo de inventário para o item. 1 = item de estoque, 2 = item de serviço. Essa é uma propriedade obrigatória.|
|bloqueou             |booliano |Especifica que as transações com o item não podem ser lançadas, por exemplo, porque o item está em quarentena. Defina como **true**se o item estiver bloqueado.|
|baseUnitOfMeasureId |GUID    |Especifica a ID da unidade de medida.             |
|baseUnitOfMeasure   |[Extra. UnitOfMeasure](../resources/dynamics-complextypes.md)|Especifica a unidade na qual o item é mantido no estoque.|
|GTIN                |numéricos |Este é o número do item comercial global.                |
|objectcategoryid      |GUID |Especifica a categoria à qual o item pertence. As categorias de item também contêm qualquer atributo de item atribuído.|
|inventory           |dígitos |Especifica quantas unidades, como peças, caixas ou latas do item estão no estoque. Somente Leitura.|
|PreçoUnitário           |dígitos |Especifica o preço de uma unidade do item na moeda especificada.|
|priceIncludesTax    |booliano |Especifica que o PreçoUnitário inclui o imposto. Defina como **true**, se PreçoUnitário incluir imposto.|
|unitCost            |dígitos |Especifica o custo por unidade do item.             |
|taxGroupId          |GUID    |Especifica a ID do grupo de impostos para o item.      |
|taxGroupCode        |numéricos |Um grupo de impostos representa um grupo de itens ou recursos de estoque sujeitos a termos de impostos idênticos.|
|lastModifiedDateTime|DateTime|A última data/hora em que o item foi modificado. Somente leitura.  |  


## <a name="relationships"></a>Relações
Um grupo de impostos (taxGroupCode) deve existir na tabela de grupos de impostos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
      "id": "GUID",
      "number": "string",
      "displayName": "string",
      "type": "string",
      "blocked": "boolean",
      "baseUnitOfMeasureId": "GUID",
      "baseUnitOfMeasure": "NAV.UnitOfMeasure",
      "gtin": "numeric",
      "itemCategoryId": "GUID",
      "inventory": "decimal",
      "unitPrice": "decimal",
      "priceIncludesTax": "boolean",
      "unitCost": "decimal",
      "taxGroupId": "GUID",
      "taxGroupCode": "string",
      "lastModifiedDateTime": "datetime"
}

```


