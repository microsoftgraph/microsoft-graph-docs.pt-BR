---
title: Criar paymentMethods
description: Cria um objeto de método de pagamento no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 64d7dac3590845f4fa4a95de9fc32829654a1d57
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473272"
---
# <a name="create-paymentmethods"></a>Criar paymentMethods

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um objeto de método de pagamento no DDynamics 365 Business Central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegada (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
```http
POST /financials/companies/{id}/paymentMethods
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho         |Valor                        |
|---------------|-----------------------------|
|Autorização  |{token} de portador. Obrigatório.    |
|Content-Type   |application/json             |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um **objeto paymentMethods.**

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará ```201 Created``` o código de resposta e um objeto **paymentMethods** no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Aqui está um exemplo de uma solicitação.

```http
POST https://graph.microsoft.com/beta/financials/companies/{id}/paymentMethods
Content-type: application/json

{
  "code": "CHECK",
  "displayName": "Check payment"
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
  "code": "CHECK",
  "displayName": "Check payment",
  "lastModifiedDateTime": "2017-03-22T08:35:48.33Z"
}

```



