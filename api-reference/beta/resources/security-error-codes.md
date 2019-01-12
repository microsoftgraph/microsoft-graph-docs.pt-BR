---
title: Respostas de erros de API de segurança do Microsoft Graph
description: Erros na API de segurança do Microsoft Graph são retornados usando o código de status HTTP 206 parcial conteúdo padrão e são fornecidos por meio de um cabeçalho de aviso.
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 52b7c375bd3e0c6a367f1150a21bb96ef84437ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921423"
---
# <a name="microsoft-graph-security-api-error-responses"></a>Respostas de erros de API de segurança do Microsoft Graph

Erros na API de segurança do Microsoft Graph são retornados usando o código de status HTTP 206 parcial conteúdo padrão e são fornecidos por meio de um cabeçalho de aviso.

## <a name="errors"></a>Erros

A API de segurança do Microsoft Graph é um serviço federado que recebe várias respostas de todos os provedores de dados. Quando um erro HTTP é recebido pelo API de segurança do Microsoft Graph, ele retornará um cabeçalho de aviso no seguinte formato:<!-- { "blockType": "ignored" } -->

```http
{Vendor}/{Provider}/{StatusCode}/{LatencyInMs}
```

Este cabeçalho do aviso será enviado apenas para os clientes quando um dos provedores de dados retorna um código de erro que não seja 2xx ou 404. Por exemplo:

- HttpStatusCode.Forbidden (403) pode ser retornado se o acesso ao recurso não é concedido.
- Se um provedor de tempo limite, HttpStatusCode.GatewayTimeout (504) é retornado no cabeçalho do aviso.
- Se um erro interno do provedor acontecer, HttpStatusCode.InternalServerError (500) é usado no cabeçalho do aviso.

Se um provedor de dados retorna 2xx ou 404, ele não será mostrado no cabeçalho do aviso porque esses códigos esperados para o sucesso ou quando os dados não são encontrados respectivamente. Em um sistema federado, um 404 não encontrado é esperado como muitas vezes, os dados somente são conhecidos por um ou vários, mas nem todos os provedores.

## <a name="example"></a>Exemplo

Um usuário solicita `security/alerts/{alert_id}`.

    Provider 1: 404 (provider does not have a record of this alert ID)
    Provider 2: 504 (provider timed out)
    Provider 3: 200 (success)
    Provider 4: 403 (customer has not licensed this provider)

Como 404 e 200 são condições esperadas, o cabeçalho do aviso contém o seguinte:

```HTTP
Warning : 199 - "{Vendor2}/{Provider 2}/504/10000",    (usual timeout limit is set at 10 seconds)
          199 - "{Vendor4}/{Provider 4}/403/10"       (Provider 4 rejected the request in 10 ms)
```

> **Observação:** Cada cabeçalho HTTP é uma coleção de subitems, para que os usuários possam enumerar o cabeçalho do aviso e verificar todos os itens.

## <a name="constraints"></a>Restrições

O `$top` parâmetro de consulta OData tem um limite de alertas de 1000 e uma combinação de `$top`  +  `$skip` consulta OData parâmetros não podem exceder 6000 alertas. Por exemplo, `/security/alerts?$top=10&$skip=5990` retornará um `200 OK` código de resposta, mas `/security/alerts?$top=10&$skip=5991` retornará um `400 Bad Request` código de resposta.

Uma solução alternativa para esse limite é usar o `$filter` parâmetro de consulta OData com o `eventDateTime` da entidade alerta da API de segurança do Microsoft Graph, usando `?$filter=eventDateTime gt {YYYY-MM-DDT00:00:00.000Z}` e substituindo o valor de data/hora com o último alerta (6000th). Você também pode definir um intervalo para o `eventDateTime`; Por exemplo, *filtro de $ alerts? = eventDateTime **gt** 2018-11 -**11**T00:00:00.000Z & eventDateTime **lt** 2018-11 -**12**T00:00:00.000Z*

## <a name="see-also"></a>Confira também

Se você estiver tendo problemas com autorização, consulte [Authorization and a API de segurança do Microsoft Graph](/graph/security-authorization).
