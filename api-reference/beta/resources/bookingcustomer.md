---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: af64f8686b1779030c0ace93b4805845c6ed3c81
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507993"
---
# <a name="bookingcustomer-resource-type"></a>tipo de recurso bookingCustomer

Namespace: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um cliente de um [bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar clientes](../api/bookingbusiness-list-customers.md) | coleção [bookingCustomer](bookingcustomer.md) | Obtenha uma lista de objetos **bookingCustomer** . |
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Criar um novo objeto **bookingCustomer** . |
|[Obter bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Atualizar um objeto **bookingCustomer** . |
|[Delete](../api/bookingcustomer-delete.md) | None |Excluir um objeto **bookingCustomer** . |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres|O nome do cliente.|
|emailAddress|String|O endereço SMTP do cliente.|
|id|String| A ID do cliente. Somente leitura.|

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
  "id": "String (identifier)"
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
