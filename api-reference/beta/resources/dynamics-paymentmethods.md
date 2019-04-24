---
title: tipo de recurso paymentMethods
description: Um objeto de método de pagamento no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 1e4cd044d4b552a9239b742efb302633524ce22b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507235"
---
# <a name="paymentmethods-resource-type"></a>tipo de recurso paymentMethods
Representa um método de pagamento no Dynamics 365 Business central, como PayPal, cartão de crédito e conta bancária.

## <a name="methods"></a>Métodos

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
|lastModifiedDateTime|DateTime|A última data/hora em que o método de pagamento foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Nenhuma

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
