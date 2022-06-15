---
title: Criar ediscoveryNoncustodialDataSource
description: Crie um novo objeto ediscoveryNoncustodialDataSource.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 5fb5dafb7fac81632697d6822d621a6e5f248ad1
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092885"
---
# <a name="create-ediscoverynoncustodialdatasource"></a>Criar ediscoveryNoncustodialDataSource
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo objeto ediscoveryNoncustodialDataSource.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) .

Você pode especificar as propriedades a seguir ao criar **um ediscoveryNoncustodialDataSource**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Datasource|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|Obrigatório. Um userSource ou siteSource. Para userSource, use "dataSource": { "@odata.type": "microsoft.graph.security.userSource", "email" : "Endereço SMTP"}.  Para a fonte do site, use "dataSource": { "@odata.type": "microsoft.graph.security.siteSource", "site@odata.bind" : "siteId" }, em que siteId pode ser derivado da URL do site, `https://contoso.sharepoint.com/sites/HumanResources`por exemplo, a solicitação do Microsoft Graph seria `https://graph.microsoft.com/v1.0/sites/contoso.sharepoint.com:/sites/HumanResources`. A ID é o primeiro GUID listado no campo ID. Como alternativa, use a webUrl diretamente, "dataSource": {"@odata.type": "microsoft.graph.security.siteSource","site": {"webUrl": `https://m365x809305.sharepoint.com/sites/Design-topsecret`}}



## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201 Created` um código de resposta [e um objeto ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_ediscoverynoncustodialdatasource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources
Content-Type: application/json

{
    "dataSource": {
        "@odata.type": "microsoft.graph.security.siteSource",
        "site": {
            "webUrl": "https://m365x809305.sharepoint.com/sites/Design-topsecret"
        }
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-ediscoverynoncustodialdatasource-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-ediscoverynoncustodialdatasource-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-ediscoverynoncustodialdatasource-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-ediscoverynoncustodialdatasource-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/noncustodialDataSources/$entity",
    "status": "active",
    "holdStatus": "notApplied",
    "createdDateTime": "2022-05-23T03:15:08.5354451Z",
    "lastModifiedDateTime": "2022-05-23T03:15:08.5354451Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "43373338343345303943344434423032",
    "displayName": "Design - top secret"
}
```
