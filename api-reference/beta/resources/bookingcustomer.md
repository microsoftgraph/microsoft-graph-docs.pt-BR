---
title: tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: cd4991b28f1dee0ba647a7f95b70817beffbef95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543861"
---
# <a name="bookingcustomer-resource-type"></a>tipo de recurso bookingCustomer

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um cliente de um [bookingBsiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar clientes](../api/bookingbusiness-list-customers.md) | coleção [bookingCustomer](bookingcustomer.md) | Obtenha uma lista de objetos **bookingCustomer** . |
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Criar um novo objeto **bookingCustomer** . |
|[Obter bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Leia as propriedades e os relacionamentos de um objeto **bookingCustomer** .|
|[Update](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Atualizar um objeto **bookingCustomer** . |
|[Excluir](../api/bookingcustomer-delete.md) | None |Excluir um objeto **bookingCustomer** . |

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingcustomer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
