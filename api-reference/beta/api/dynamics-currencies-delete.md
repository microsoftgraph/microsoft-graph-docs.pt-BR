---
title: Excluir moedas
description: Exclui um objeto currency no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: b9f6c729dc97d523952454978afc056c05c354c5
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473151"
---
# <a name="delete-currencies"></a>Excluir moedas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua um objeto currency do Dynamics 365 Business Central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegada (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
```
DELETE /financials/companies/{id}/currencies/{id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Cabeçalho|Valor|
|------|-----|
|Autorização  |{token} de portador. Obrigatório. |
|If-Match       |Obrigatório. Quando esse header de solicitação for incluído e a eTag fornecida não corresponder à marca atual nas moedas **,** as moedas **não** serão
 atualizado. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Este é um exemplo da solicitação.

```http
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/currencies/{id}
```

**Response** 

Veja a seguir um exemplo da resposta. 

```http
HTTP/1.1 204 No Content
```


