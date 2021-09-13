---
title: Respostas de Graph de erro da API de Segurança da Microsoft
description: Os erros na API de Segurança do Microsoft Graph são retornados usando o código de status de Conteúdo Parcial HTTP 206 padrão e são entregues por meio de um cabeçalho de aviso.
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 674ccf9817d01f48a0db40906ba2cfd656ff3dfe
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080566"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Respostas de Graph de erro da API de Segurança da Microsoft

Namespace: microsoft.graph

Os erros na API de Segurança do Microsoft Graph são retornados usando o código de status de Conteúdo Parcial HTTP 206 padrão e são entregues por meio de um cabeçalho de aviso.

## <a name="errors"></a>Erros

A API Graph de Segurança da Microsoft é um serviço federado que recebe várias respostas de todos os provedores de dados. Quando um erro HTTP é recebido pela API de Segurança do Microsoft Graph, ele enviará de volta um cabeçalho de aviso no seguinte formato:
<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Esse header de aviso só é enviado de volta para clientes quando um dos provedores de dados retorna um código de erro diferente de 2xx ou 404. Por exemplo:

- HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não for concedido.
- Se um provedor se estime, HttpStatusCode.GatewayTimeout (504) será retornado no cabeçalho de aviso.
- Se ocorrer um erro de provedor interno, HttpStatusCode.InternalServerError (500) será usado no cabeçalho de aviso.

Se um provedor de dados retornar 2xx ou 404, ele não será mostrado no header de aviso porque esses códigos são esperados para sucesso ou quando os dados não são encontrados, respectivamente. Em um sistema federado, um 404 não encontrado é esperado quantas vezes os dados são conhecidos apenas por um ou vários provedores, mas não todos.

## <a name="example"></a>Exemplo

Um usuário solicita `security/alerts/{alert_id}` .

```
Provider 1: 404 (provider does not have a record of this alert ID)
Provider 2: 504 (provider timed out)
Provider 3: 200 (success)
Provider 4: 403 (customer has not licensed this provider)
```

Como as condições 404 e 200 são esperadas, o header de aviso contém o seguinte:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitens, para que os usuários possam enumerar o cabeçalho Aviso e verificar todos os itens.

## <a name="threat-indicator-bulk-action-errors"></a>Erros de ação em massa do indicador de ameaça

Ações em massa (criar, atualizar, excluir) podem gerar dois códigos de erro possíveis diferentes:

- Um código de erro 400 indica que o corpo fornecido teve um erro durante a serialização.
- Um código de erro 206 indica que uma ou mais das ações em massa falharam quando ela foi federada para seu provedor. A resposta conterá dados de sucesso/erro dos provedores individuais para cada indicador de inteligência de ameaça. Ao [contrário dos alertas,](/graph/api/resources/security-api-overview?view=graph-rest-1.0#alerts)todas as informações de erro potenciais serão contidas no corpo da resposta para ações em massa [tiIndicator.](/graph/api/resources/security-api-overview?view=graph-rest-beta#threat-indicators-preview)

## <a name="constraints"></a>Restrições

O `$top` parâmetro de consulta OData tem um limite de 1000 alertas. É recomendável incluir apenas o `$top` e não o `$skip` na primeira consulta OBTER. Você pode usar `@odata.nextLink` para paginação. Se você precisar usar o `$skip`, ele tem um limite de 500 alertas. Por exemplo, `/security/alerts?$top=10&$skip=500` retornará um código de resposta `200 OK`, mas `/security/alerts?$top=10&$skip=501` retornará um código de resposta `400 Bad Request`. Para obter mais informações, consulte as [respostas de erro da API de segurança do Microsoft Graph](../resources/security-error-codes.md).

Uma solução alternativa para esse limite é usar o parâmetro de consulta OData com a entidade de alerta da API de Segurança do Microsoft Graph, usando e substituindo o valor dateTime pelo último `$filter` `eventDateTime` alerta `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` (1500th). Você também pode definir um intervalo para `eventDateTime` ; por exemplo, `alerts?$filter=eventDateTime **gt** 2018-11-**11**T00:00:00.000Z&eventDateTime **lt** 2018-11-**12**T00:00:00.000Z` .

## <a name="see-also"></a>Também confira

Se você estiver tendo problemas com autorização, consulte Autorização e a API Graph [Segurança da Microsoft.](/graph/security-authorization)


