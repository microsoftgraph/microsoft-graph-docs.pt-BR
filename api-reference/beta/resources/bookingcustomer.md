---
title: Tipo de recurso bookingCustomer
description: Representa um cliente de um bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 7e4c31ec68cdda121dcb1f7954faa742746271fc
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160641"
---
# <a name="bookingcustomer-resource-type"></a>Tipo de recurso bookingCustomer

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um cliente de [um bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar clientes](../api/bookingbusiness-list-customers.md) | [coleção bookingCustomer](bookingcustomer.md) | Obtenha uma lista de **objetos bookingCustomer** . |
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Crie um novo **objeto bookingCustomer** . |
|[Obter bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Leia as propriedades e as relações de um **objeto bookingCustomer** .|
|[Atualizar](../api/bookingcustomer-update.md) | Nenhum(a)  |Atualize **um objeto bookingCustomer** . |
|[Excluir](../api/bookingcustomer-delete.md) | Nenhuma |Exclua **um objeto bookingCustomer** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|addresses|[coleção physicalAddress](../resources/physicaladdress.md)|Endereços associados ao cliente, incluindo endereços domésticos, comerciais e outros.|
|displayName|Cadeia de caracteres|O nome do cliente.|
|emailAddress|String|O endereço SMTP do cliente.|
|id|Cadeia de caracteres| A ID do cliente. Somente leitura.|
|telefones|Coleção [phone](../resources/phone.md)|Telefone números associados ao cliente, incluindo números domésticos, comerciais e móveis.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingCustomer"
}-->

```json
{
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "addresses": [
    {
      "@odata.type": "microsoft.graph.physicalAddress"
    }
  ],
  "phones": [
    {
      "@odata.type": "microsoft.graph.phone"
    }
  ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingCustomer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


