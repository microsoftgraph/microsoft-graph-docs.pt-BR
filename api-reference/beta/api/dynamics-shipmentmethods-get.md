---
title: Obter shipmentMethods
description: Obtém um objeto de método de remessa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 956cc594d7dd4912f5a9c7e5f48c5528c235999f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955992"
---
# <a name="get-shipmentmethods"></a>Obter shipmentMethods
Recupere as propriedades e os relacionamentos de um objeto de método de remessa para o Dynamics 365 Business central.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão |Permissões (da com menos para a com mais privilégios)|
|:---------------|:------------------------------------------|
|Delegado (conta corporativa ou de estudante)|Financials.ReadWrite.All |
|Delegado (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Financials.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

```
GET /financials/companies('{id}')/shipmentMethods('{id}')
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|------|-----|
|Autorização  |{token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **shipmentMethods** no corpo da resposta.

## <a name="example"></a>Exemplo

**Solicitação**

Este é um exemplo da solicitação.
```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/shipmentMethods('{id}')
```

**Resposta**

Veja a seguir um exemplo da resposta. 

> **Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

```json
{
  "id": "id-value",
  "code": "PICKUP",
  "displayName": "Pickup at Location",
  "lastModifiedDateTime": "2017-03-15T02:20:57.09Z"
}
```

