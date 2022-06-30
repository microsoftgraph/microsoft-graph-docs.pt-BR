---
title: Criar externalGroup
description: Crie um novo objeto externalGroup.
author: sacampbe-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 7d406c63f9974b023a97a119533cb2db29732bad
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443470"
---
# <a name="create-externalgroup"></a>Criar externalGroup
Namespace: microsoft.graph.externalConnectors



Crie um novo [objeto externalGroup](../resources/externalconnectors-externalgroup.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte                               |
| Aplicativo                            | ExternalItem.ReadWrite.OwnedBy, ExternalItem.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /external/connections/{connectionsId}/groups
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                 |
|:--------------|:----------------------------|
| Autorização | {token} de portador. Obrigatório.   |
| Content-Type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do **objeto externalGroup** .

Você pode especificar as propriedades a seguir ao criar um **externalGroup**.

| Propriedade    | Tipo   | Descrição                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| id          | Cadeia de caracteres | A ID exclusiva do grupo externo dentro de uma conexão. Ele deve ser alfanumérico e pode ter até 128 caracteres. Obrigatório. |
| displayName | String | O nome amigável do grupo externo. Opcional.                                                                      |
| description | Cadeia de caracteres | A descrição do grupo externo. Opcional.                                                                         |



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `201 Created` de resposta e um **objeto externalGroup** no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_externalgroup_from_connection"
}
-->

``` http
POST https://graph.microsoft.com/v1.0/external/connections/contosohr/groups
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-externalgroup-from-connection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-externalgroup-from-connection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-externalgroup-from-connection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-externalgroup-from-connection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-externalgroup-from-connection-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-externalgroup-from-connection-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "31bea3d537902000",
  "displayName": "Contoso Marketing",
  "description": "The product marketing team"
}
```
