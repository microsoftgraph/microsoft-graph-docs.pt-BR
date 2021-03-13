---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8610c51922989d96f455073ea824c258d6d454ba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774796"
---
# <a name="update-teamsapp"></a>Atualizar teamsApp

Namespace: microsoft.graph

Atualize [um aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams. Para atualizar um aplicativo, a **propriedade distributionMethod** para o aplicativo deve ser definida como `organization` .

Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos de locatário).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Somente administradores globais podem chamar essa API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegada (conta corporativa ou de estudante)     | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a>Parâmetros de consulta

|Propriedade|Tipo|Descrição|
|----|----|----|
|requiresReview| Booliano | Esse parâmetro de consulta opcional aciona o processo de revisão do aplicativo. Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão. Se os usuários quiserem solicitar uma revisão antes da publicação, eles deverão definir  `requiresReview` como `true` . Um usuário com privilégios de administrador pode optar por não definir ou definir o valor como e o aplicativo será considerado aprovado e `requiresReview` `false`  publicará instantaneamente.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | application/zip. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua uma carga de manifesto zip do Teams. Para obter detalhes, consulte [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)

>**Observação:** Use a ID retornada da chamada Lista [de](./appcatalogs-list-teamsapps.md) aplicativos publicados para fazer referência ao aplicativo que você gostaria de atualizar. Não use a ID do manifesto do pacote do aplicativo zip.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a>Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams

#### <a name="request"></a>Solicitação

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Para obter detalhes sobre o arquivo zip do aplicativo Teams, consulte [Create app package](/microsoftteams/platform/concepts/apps/apps-package).
<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a>Exemplo 2: atualizar uma nova versão de um aplicativo existente para revisão de administrador antes da publicação no catálogo de locatários atual

#### <a name="request"></a>Solicitação

<!-- markdownlint-disable MD034 -->


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e o par `201 Created` chave/valor `publishingState` : no corpo da `submitted` resposta. *Consulte* [teamsappdefinition](../resources/teamsappdefinition.md).

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```
