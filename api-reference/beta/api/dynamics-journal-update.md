---
title: Atualizar diários
description: Atualiza um objeto Journal no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 7f98f063e6c796d15adc141e58d761ad7de0f154
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791481"
---
# <a name="update-journals"></a>Atualizar diários
Atualizar as propriedades de um objeto Journal para o Dynamics 365 Business central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegado (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

```
PATCH /financials/companies/{id}/journals/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho        |Valor                    |
|--------------|-------------------------|
|Autorização |{token} de portador. Obrigatório.|
|Content-Type  |application/json         |
|If-Match      |Obrigatório. Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual dos **diários**, os **diários** não serão atualizados. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **Journals** atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Este é um exemplo da solicitação.
```json
PATCH https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}
Content-type: application/json

{
  "code": "EXPENSE",
  "displayName": "Expense Batch"
}
```

**Resposta**

Veja a seguir um exemplo da resposta. 

> **Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "code": "EXPENSE",
  "displayName": "Expense Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```

