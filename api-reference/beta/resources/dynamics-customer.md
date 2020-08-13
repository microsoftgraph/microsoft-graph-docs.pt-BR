---
title: tipo de recurso clientes
description: Representa um cliente no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5abe6b5fcf56544d587edbedf20f22594be0cdd0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504710"
---
# <a name="customers-resource-type"></a>tipo de recurso clientes

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um cliente no Dynamics 365 Business central.

## <a name="methods"></a>Métodos

| Método                                              |Tipo de retorno| Descrição      |
|:----------------------------------------------------|:----------|:-----------------|
|[Obter clientes](../api/dynamics-customer-get.md)      |Eles   |Obtém um cliente.   |
|[Criar clientes](../api/dynamics-create-customer.md)|Eles   |Cria um cliente.|
|[Atualizar clientes](../api/dynamics-customer-update.md)|Eles   |Atualiza um cliente.|
|[Excluir clientes](../api/dynamics-customer-delete.md)|Nenhuma        |Exclui um cliente.|

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo     |Descrição|
|:------------|:---------|:----------|
|id           |GUID      |A ID exclusiva do item. Não editável.|
|number       |cadeia de caracteres    |O número do cliente.|
|displayName  |cadeia de caracteres    |Especifica o nome do cliente. Esse nome aparecerá em todos os documentos de vendas do cliente.|
|type         |string    |Especifica o tipo de cliente, pode ser "empresa" ou "pessoa".|
|address      |[Extra. Address](../resources/dynamics-complextypes.md)|Especifica o endereço do cliente. Esse endereço aparecerá em todos os documentos de vendas do cliente.|
|phoneNumber  |cadeia de caracteres    |Especifica o número de telefone do cliente.|
|email        |cadeia de caracteres    |Especifica o endereço de email do cliente.|
|site      |cadeia de caracteres    |Especifica o endereço da home page do cliente.|
|taxLiable    |booliano   |Especifica se o cliente ou fornecedor é responsável pelo imposto sobre vendas. Defina como **true** se o cliente for responsável por impostos.|
|taxAreaId    |GUID      |Especifica a área de impostos à qual o cliente pertence.|
|taxAreaDisplayName|cadeia de caracteres|Especificou o nome de exibição da área de impostos à qual o cliente pertence.|
|taxRegistrationNumber|Cadeia de caracteres, tamanho máximo 20|Especificado o número de registro de imposto do cliente.|
|CurrencyID   |GUID      |Especifica a moeda usada pelo cliente.|
|currencyCode |numéricos   |O código de moeda padrão para o cliente.|
|paymentTermsId|GUID     |Especifica qual termo de pagamento o cliente utiliza.|
|paymentMethodId|GUID    |Especifica qual método de pagamento o cliente utiliza.|
|shipmentMethodId|GUID   |Especifica o método de remessa que o cliente usa.|
|bloqueou      |cadeia de caracteres    |Especifica que as transações com o cliente não podem ser lançadas. Defina como **todos**, se o cliente estiver bloqueado, defina como em branco se não for bloqueado.|
|carga      |numéricos   |Especifica o valor do pagamento que o cliente está procurando para vendas concluídas. Esse valor também é conhecido como o saldo do cliente. Somente Leitura.|
|overdueAmount|numéricos   |Especifica o valor vencido do cliente.|
|totalSalesExcludingTax|numéricos|Especifica o valor total de vendas excluindo o imposto do cliente.|
|lastModifiedDateTime|datetime|O último DateTime que o cliente foi modificado. Somente leitura.|  


## <a name="relationships"></a>Relações
Uma moeda (currencyCode) deve existir na tabela moedas.

Um termo de pagamento (paymentTerms) deve existir na tabela de condições de pagamento.

Um método de remessa (shipmentMethod) deve existir na tabela do método de remessa.

Um método de pagamento (paymentMethod) deve existir na tabela de métodos de pagamento.

Uma área de impostos (taxArea) deve existir na tabela de área de impostos.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```

