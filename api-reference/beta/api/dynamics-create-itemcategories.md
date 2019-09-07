---
title: Criar categorias de categoria
description: Cria um objeto de categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: cf44a683f79192d02ffe87f57b0a9d5d92bc0f27
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791992"
---
# <a name="create-itemcategories"></a>Criar categorias de categoria
Criar um objeto de categoria de item Dynamics 365 Business central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegado (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
```
POST /financials/companies/{id}/itemCategories
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho       |Valor                    |
|-------------|-------------------------|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type |application/json         |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto **myCategories** .

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **myCategories** no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Veja a seguir um exemplo de uma solicitação.

```json
POST https://graph.microsoft.com/beta/financials/companies/{id}/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

**Resposta**

Veja a seguir um exemplo da resposta. 

> **Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




