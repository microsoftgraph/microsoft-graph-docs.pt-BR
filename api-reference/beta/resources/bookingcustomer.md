---
title: Tipo de recurso bookingCustomer
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 3d5eff9d0add4a0840e864b9f4caf1730be98e5a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696228"
---
# <a name="bookingcustomer-resource-type"></a>Tipo de recurso bookingCustomer

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um cliente de [um bookingBusiness](bookingbusiness.md).


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar clientes](../api/bookingbusiness-list-customers.md) | [coleção bookingCustomer](bookingcustomer.md) | Obter uma lista de **objetos bookingCustomer.** |
|[Criar bookingCustomer](../api/bookingbusiness-post-customers.md) | [bookingCustomer](bookingcustomer.md) | Crie um novo **objeto bookingCustomer.** |
|[Obter bookingCustomer](../api/bookingcustomer-get.md) | [bookingCustomer](bookingcustomer.md) |Leia as propriedades e as relações de um **objeto bookingCustomer.**|
|[Atualizar](../api/bookingcustomer-update.md) | [bookingCustomer](bookingcustomer.md) |Atualize um **objeto bookingCustomer.** |
|[Excluir](../api/bookingcustomer-delete.md) | Nenhum |**Exclua um objeto bookingCustomer.** |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String|O nome do cliente.|
|emailAddress|String|O endereço SMTP do cliente.|
|id|String| A ID do cliente. Apenas leitura.|
|addresses|[Coleção physicalAddress](../resources/physicaladdress.md)|Endereços associados ao cliente, incluindo home, business e outros endereços.|
|telefones|Coleção [phone](../resources/phone.md)|Telefone números associados ao cliente, incluindo números fixos, comerciais e móveis.|

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


