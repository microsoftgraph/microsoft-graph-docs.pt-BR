---
title: Obter synchronizationtemplate
description: Recupere um modelo de sincronização por seu identificador.
localization_priority: Normal
ms.openlocfilehash: 982727fa54f1b6f83d7acf382f0ccacdad72b7ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335538"
---
# <a name="get-synchronizationtemplate"></a>Obter synchronizationtemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere um modelo de sincronização por seu identificador.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     |Directory.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft) |Sem suporte.|
|Aplicativo                            |Sem suporte.| 

### <a name="http-request"></a>Solicitação HTTP

```http
GET applications/{id}/synchronization/templates/{templateId}
GET servicePrincipals/{id}/synchronization/templates/{templateId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Tipo    | Descrição|
|:---------------|:--------|:-----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [synchronizationtemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.

### <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/templates/Slack
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo de uma resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas em uma chamada real.

```http
HTTP/1.1 200 OK
{
    "id": "Slack",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
        }
}
```
