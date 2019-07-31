---
title: tipo de recurso customerPaymentJournals
description: Um diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0791fe2b8c36bdff535f7fc56dea54abe1632647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973629"
---
# <a name="customerpaymentsjournals-resource-type"></a>tipo de recurso customerPaymentsJournals
Representa um diário de pagamento do cliente no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método               | Tipo de retorno             |Descrição                      |
|:---------------------|:------------------------|:--------------------------------|
|[Obter customerPaymentJournals](../api/dynamics-customerpaymentsjournal-get.md)      |customerPaymentJournals|Obtém um diário de pagamentos do cliente.   |
|[Postar customerPaymentJournals](../api/dynamics-create-customerpaymentsjournal.md)  |customerPaymentJournals|Cria um diário de pagamentos do cliente.|
|[Patch customerPaymentJournals](../api/dynamics-customerpaymentsjournal-update.md) |customerPaymentJournals|Atualiza um diário de pagamento do cliente.|
|[Excluir customerPaymentJournals](../api/dynamics-customerpaymentsjournal-delete.md)|none                     |Exclui um diário de pagamento do cliente.|

## <a name="properties"></a>Propriedades
| Propriedade           | Tipo                  |Descrição                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |A ID exclusiva do diário de pagamento do cliente. Não editável.           |
|código                |Cadeia de caracteres, tamanho máximo 10| O código do diário de pagamento do cliente.                             |
|displayName         |Cadeia de caracteres, tamanho máximo 50| O nome de exibição do diário de pagamentos do cliente.                     |
|lastModifiedDateTime|DateTime               |O último DateTime que o diário de pagamentos do cliente foi modificado. Somente leitura.|

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

