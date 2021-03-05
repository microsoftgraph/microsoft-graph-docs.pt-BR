---
title: Criar paymentTerms
description: Cria um objeto de termos de pagamento no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 0f7df8cca531210795dcdade8725bbbf312484c6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473270"
---
# <a name="create-paymentterms"></a>Criar paymentTerms

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um objeto de termos de pagamento no Dynamics 365 Business Central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegada (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
```http
POST /financials/companies/{id}/paymentTerms
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|---------------|-----------------------------|
|Autorização  |{token} de portador. Obrigatório.    |
|Content-Type   |application/json             |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de **um objeto paymentTerms.**

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **paymentTerms** no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Aqui está um exemplo de uma solicitação.

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentTerms
Content-type: application/json

{
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false
}
```

**Response**

Veja a seguir um exemplo da resposta. 

> **Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "7 DAYS",
  "displayName": "Net 7 days",
  "dueDateCalculation": "7D",
  "discountDateCalculation": "",
  "discountPercent": 0,
  "calculateDiscountOnCreditMemos": false,
  "lastModifiedDateTime": "2017-03-03T02:14:32Z"
}

```


