---
title: Respostas de erro da API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status de conteúdo parcial HTTP 206, e são entregues por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: c36cf3be4cf24a2831918acd994a36bbcfc9e489
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988923"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Respostas de erro da API de segurança do Microsoft Graph

Namespace: microsoft.graph

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

Um usuário solicita `security/alerts/{alert_id}` .

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

Como 404 e 200 são condições esperadas, o cabeçalho de aviso contém o seguinte:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitens, de forma que os usuários possam enumerar o cabeçalho de aviso e verificar todos os itens.

## <a name="threat-indicator-bulk-action-errors"></a>Erros de ação em massa do indicador de ameaça

As ações em massa (criar, atualizar, excluir) podem gerar dois códigos de erro potenciais diferentes:

- Um código de erro 400 indica que o corpo fornecido teve um erro durante a serialização.
- Um código de erro 206 indica que uma ou mais ações em massa falharam quando foram federadas no provedor. A resposta conterá dados de sucesso/erro dos provedores individuais para cada indicador de inteligência de ameaças. Ao contrário dos [alertas](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts), todas as informações de erro em potencial serão contidas no corpo da resposta para ações em massa [tiIndicator](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview) .

## <a name="constraints"></a>Restrições

O `$top` parâmetro de consulta OData tem um limite de 1000 alertas. É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER. Você pode usar `@odata.nextLink` para paginação. Se você precisar usar o `$skip`, ele tem um limite de 500 alertas. Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`. Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

Uma solução alternativa para esse limite é usar o `$filter` parâmetro de consulta OData com a `eventDateTime` entidade de alerta da API de segurança do Microsoft Graph, usando `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` e substituindo o valor DateTime pelo último alerta (1500th). Você também pode definir um intervalo para o `eventDateTime` ; por exemplo, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` .

## <a name="see-also"></a>Confira também

Se você estiver tendo problemas com a autorização, confira [autorização e a API de segurança do Microsoft Graph](/graph/security-authorization).


