---
title: Respostas de erro da API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: d1a65eb214fee21389b7d6c78c10a0d9b9d0e4ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446923"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Respostas de erro da API de segurança do Microsoft Graph

Namespace: Microsoft. Graph

Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.

## <a name="errors"></a>Erros

A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados. Quando um erro HTTP é recebido pela API de segurança do Microsoft Graph, ele envia de volta um cabeçalho de aviso no seguinte formato:
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Esse cabeçalho de aviso é enviado de volta aos clientes quando um dos provedores de dados retorna um código de erro diferente de 2xx ou 404. Por exemplo:

- HttpStatusCode. proibido (403) poderá ser retornado se o acesso ao recurso não for concedido.
- Se um provedor expirar, HttpStatusCode. GatewayTimeout (504) será retornado no cabeçalho de aviso.
- Se ocorrer um erro de provedor interno, HttpStatusCode. InternalServerError (500) será usado no cabeçalho de aviso.

Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no cabeçalho de aviso porque esses códigos são esperados para êxito ou quando os dados não são encontrados, respectivamente. Em um sistema federado, um 404 não encontrado é esperado quantas vezes os dados são conhecidos apenas por um ou vários provedores.

## <a name="example"></a>Exemplo

Um usuário solicita `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Como 404 e 200 são condições esperadas, o cabeçalho de aviso contém o seguinte:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitens, de forma que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.

## <a name="constraints"></a>Restrições

O `$top` parâmetro de consulta OData tem um limite de 1000 alertas. É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER. Você pode usar `@odata.nextLink` para paginação. Se você precisar usar o `$skip`, ele tem um limite de 500 alertas. Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`. Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

Um workaaround para esse limite é usar o `$filter` parâmetro de consulta OData com a `eventDateTime` entidade de alerta da API de segurança do Microsoft Graph, usando `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` e substituindo o valor DateTime pelo último alerta (1500th). Você também pode definir um intervalo para o `eventDateTime`; por exemplo, *alertas? $Filter = eventDateTime **gt** 2018-11-**11**T00:00:00.000 z&eventDateTime **lt** 2018-11-**12**T00:00:00.000 z*

## <a name="see-also"></a>Confira também

Se você estiver tendo problemas com a autorização, confira [autorização e a API de segurança do Microsoft Graph](/graph/security-authorization).
