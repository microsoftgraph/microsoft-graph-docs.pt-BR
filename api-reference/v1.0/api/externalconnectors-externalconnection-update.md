---
title: Atualizar externalConnection
description: Atualize as propriedades de um objeto externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: c418efb3794cb30040b59211be741bd14ad7d306
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559264"
---
# <a name="update-externalconnection"></a>Atualizar externalConnection

Namespace: microsoft.graph.externalConnectors

Atualize as propriedades de [um objeto externalConnection.](../resources/externalconnectors-externalconnection.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Sem suporte. |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Application                            | ExternalConnection.ReadWrite.OwnedBy |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /external/connections/{connectionsId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades a seguir podem ser atualizadas.

| Propriedade      | Tipo                                           | Descrição |
|:--------------|:-----------------------------------------------|:------------|
| configuração | [microsoft.graph.externalConnectors.configuration](../resources/externalconnectors-configuration.md) | Especifica IDs de aplicativo adicionais que têm permissão para gerenciar a conexão e indexar conteúdo na conexão. |
| description   | Cadeia de caracteres                                         | Descrição da conexão exibida no Centro de administração do Microsoft 365. |
| name          | Cadeia de caracteres                                         | O nome de exibição da conexão a ser exibida no Centro de administração do Microsoft 365. Comprimento máximo de 128 caracteres. |


## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "update_externalconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/external/connections/contosohr
Content-type: application/json

{
  "name": "Contoso HR Service Tickets",
  "description": "Connection to index HR service tickets"
}
```


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta
<!-- markdownlint-enable MD024 -->

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
