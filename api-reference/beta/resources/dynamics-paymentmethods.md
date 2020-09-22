---
title: tipo de recurso paymentMethods
description: Um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: b30f97166625d45eba1a78342c219cbb74f42a8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013741"
---
# <a name="paymentmethods-resource-type"></a>tipo de recurso paymentMethods

Namespace: Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um método de pagamento no Dynamics 365 Business central, como PayPal, cartão de crédito e conta bancária.

## <a name="methods"></a>Methods

| Método                                                          | Tipo de retorno  |Descrição             |
|:----------------------------------------------------------------|:-------------|:-----------------------|
|[Obter paymentMethods](../api/dynamics-paymentmethods-get.md)      |paymentMethods|Obtém um objeto de método de pagamento.   |
|[Postar paymentMethods](../api/dynamics-create-paymentmethods.md)  |paymentMethods|Cria um objeto de método de pagamento.|
|[Patch paymentMethods](../api/dynamics-paymentmethods-update.md) |paymentMethods|Atualiza um objeto de método de pagamento.|
|[Excluir paymentMethods](../api/dynamics-paymentmethods-delete.md)|Nenhuma          |Exclui um objeto de método de pagamento.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo   |Descrição                                                  |
|:-------------------|:-------|:------------------------------------------------------------|
|id                  |GUID    |A ID exclusiva do paymentMethods. Não editável.           |
|código                |cadeia de caracteres  |Especifica o código do método de pagamento.                           |
|displayName         |string  |Especifica o nome de exibição do método de pagamento.                   |
|lastModifiedDateTime|datetime|A última data/hora em que o método de pagamento foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do paymentMethods.


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}

```


