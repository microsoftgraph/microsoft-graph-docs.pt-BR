---
title: tipo de recurso customerPayments
description: Um objeto Customer Payments no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bd990ea9778ada7d43c9b8192d77cf8af618909b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504633"
---
# <a name="customerpayments-resource-type"></a>tipo de recurso customerPayments

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um pagamento de cliente no Dynamics 365 Business central. Um pagamento de cliente é inserido como uma linha em um diário de pagamento do cliente.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter customerPayments](../api/dynamics-customerpayment-get.md)|customerPayments|Obtém um pagamento de cliente.|
|[Postar customerPayments](../api/dynamics-create-customerpayment.md)|customerPayments|Cria um pagamento de cliente.|
|[Patch customerPayments](../api/dynamics-customerpayment-update.md)|customerPayments|Atualiza um pagamento de cliente.|
|[Excluir customerPayments](../api/dynamics-customerpayment-delete.md)|nenhuma|Exclui um pagamento de cliente.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo    |Descrição|
|:-------------|:--------|:----------|
|id|GUID|A ID exclusiva do pagamento do cliente. Não editável.|
|journalDisplayName|string|O diário de pagamentos do cliente no qual o registro de pagamento é uma linha.|
|lineNumber|inteiro|O número do pagamento do cliente.|
|Box|GUID|A ID exclusiva do cliente ao qual o pagamento está relacionado.|
|customerNumber|Cadeia de caracteres, tamanho máximo 20|O número do cliente ao qual o pagamento está relacionado.|
|ContactID|Cadeia de caracteres, tamanho máximo 250|A ID de contato do Exchange para o cliente específico. Se uma ID de cliente não for especificada, usaremos a ID de contato para encontrá-la.|
|postingDate|data|A data em que o pagamento do cliente é lançado.|
|documentNumber|Cadeia de caracteres, tamanho máximo 20|Especifica um número de documento para o pagamento do cliente.|
|externalDocumentNumber|Cadeia de caracteres, tamanho máximo 20|Especifica um número de documento externo para o pagamento do cliente.|
|quantia|dígitos|Especifica o valor total (incluindo o IVA) que o pagamento do cliente consiste.|
|appliesToInvoiceId|GUID|A identificação exclusiva da fatura à qual o pagamento está relacionado.|
|appliesToInvoiceNumber|Cadeia de caracteres, tamanho máximo 20|O número da fatura à qual o pagamento está relacionado.|
|description|Cadeia de caracteres, tamanho máximo 50|A descrição do pagamento do cliente, fornecida pelo usuário ou pela autocriação.|
|comment|Cadeia de caracteres, tamanho máximo 250|Um comentário especificado pelo usuário no pagamento do cliente.|
|lastModifiedDateTime|datetime|O último DateTime que o pagamento do cliente foi modificado. Somente leitura.|


## <a name="relationships"></a>Relações
Um pagamento de cliente é uma subpágina de um diário de pagamento de cliente. Ele não pode ser acessado diretamente.

Um pagamento de cliente pode ser uma "entidade pai" das linhas de dimensão.

Um cliente (customerId) deve existir na tabela Customers.

Uma fatura (appliesToInvoiceId) deve existir na tabela faturas de vendas.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

