---
title: Criar custodiante unifiedGroupSource
description: Crie um novo objeto unifiedGroupSource custodiante.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 837d9f682fe4a3f177affa8fd6056cda4b6f47a8
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945118"
---
# <a name="create-custodian-unifiedgroupsource"></a>Criar custodiante unifiedGroupSource
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto unifiedGroupSource](../resources/security-unifiedgroupsource.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto unifiedGroupSource](../resources/security-unifiedgroupsource.md) .

Você pode especificar as propriedades a seguir ao criar **um unifiedGroupSource**.

>**Nota:** O **grupo** ou **group@odata.bind** é necessário para criar um **unifiedGroupSource**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|includedSources|microsoft.graph.ediscovery.sourceType|Especifica quais fontes estão incluídas neste grupo. Os valores possíveis são: `mailbox` e `site`.|
|group|Cadeia de caracteres|Especifica o endereço de email do grupo. Para obter o endereço de email de um grupo, use [Grupos de lista ou](../api/group-list.md) [Obter grupo](../api/group-get.md). Em seguida, você pode consultar pelo nome do grupo usando `$filter`; por exemplo, `https://graph.microsoft.com/v1.0/groups?$filter=displayName eq 'secret group'&$select=mail,id,displayName`.|
|group@odata.bind|Cadeia de caracteres|ID do grupo. Você pode obter isso da mesma maneira que obtém o grupo. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto unifiedGroupSource](../resources/security-unifiedgroupsource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-unifiedgroupsource-with-group-smtp-address"></a>Exemplo 1: Criar unifiedGroupSource com o endereço SMTP do grupo
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}/custodian/unifiedGroupSources
Content-Type: application/json

{
    "group": {
        "mail": "SOCTeam@M365x809305.onmicrosoft.com"
    },
    "includedSources": "mailbox, site"
}
```


#### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.unifiedGroupSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/1ce58bf6-e0fd-403d-a655-312a838110cf",
    "displayName": "SOC Team (Mailbox)",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "holdStatus": "applied",
    "id": "1ce58bf6-e0fd-403d-a655-312a838110cf",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```

### <a name="example-2-create-unifiedgroupsource-with-groupodatabind"></a>Exemplo 2: Criar unifiedGroupSource com group@odata.bind
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_unifiedgroupsource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources
Content-Type: application/json

{
    "group@odata.bind": "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610",
    "includedSources": "mailbox"
}
```


#### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.unifiedGroupSource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610",
    "displayName": "Finance Team (Mailbox)",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "holdStatus": "applied",
    "id": "93f90172-fe05-43ea-83cf-ff785a40d610",
    "includedSources": "mailbox",
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```
