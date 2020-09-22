---
title: tipo de recurso customerPaymentJournals
description: Um diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a6fc1cf1541ebfbcf514de3005c7a89961531568
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071350"
---
# <a name="customerpaymentsjournals-resource-type"></a>tipo de recurso customerPaymentsJournals

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um diário de pagamento do cliente no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método               | Tipo de retorno             |Descrição                      |
|:---------------------|:------------------------|:--------------------------------|
|[Obter customerPaymentJournals](../api/dynamics-customerpaymentsjournal-get.md)      |customerPaymentJournals|Obtém um diário de pagamentos do cliente.   |
|[Postar customerPaymentJournals](../api/dynamics-create-customerpaymentsjournal.md)  |customerPaymentJournals|Cria um diário de pagamentos do cliente.|
|[Patch customerPaymentJournals](../api/dynamics-customerpaymentsjournal-update.md) |customerPaymentJournals|Atualiza um diário de pagamento do cliente.|
|[Excluir customerPaymentJournals](../api/dynamics-customerpaymentsjournal-delete.md)|Nenhuma                     |Exclui um diário de pagamento do cliente.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |A ID exclusiva do diário de pagamento do cliente. Não editável.           |
|código                |Cadeia de caracteres, tamanho máximo 10| O código do diário de pagamento do cliente.                             |
|displayName         |Cadeia de caracteres, tamanho máximo 50| O nome de exibição do diário de pagamentos do cliente.                     |
|lastModifiedDateTime|datetime               |O último DateTime que o diário de pagamentos do cliente foi modificado. Somente leitura.|

## <a name="relationships"></a>Relações

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```



