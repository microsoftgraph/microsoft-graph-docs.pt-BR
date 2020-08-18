---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 31f7b40b8f6c1f6de1fcaf6122c4311e5a65d016
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792139"
---
# <a name="update-teamsapp"></a>Atualizar teamsApp

Namespace: microsoft.graph

Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams. Para atualizar um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .

Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

>**Observação:** Somente os administradores globais podem chamar esta API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegada (conta corporativa ou de estudante)     | AppCatalog. ReadWrite. All, Directory. ReadWrite. All |
| Delegada (conta corporativa ou de estudante) | AppCatalog. Submit|
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
|requiresReview| Booliano | Esse parâmetro de consulta opcional dispara o processo de revisão do aplicativo. Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão. Se os usuários desejarem solicitar uma revisão antes da publicação, eles devem  `requiresReview` ser definidos como `true` . Um usuário com privilégios de administrador pode optar por não definir `requiresReview` ou definir o valor como `false`  e o aplicativo será considerado aprovado e publicar instantaneamente.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | Application/zip. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua uma carga de manifesto zip do teams. Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)

>**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja atualizar. Não use a ID do manifesto do pacote de aplicativos zip.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a>Exemplo 1: atualizar um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams

### <a name="request"></a>Solicitação

<!-- markdownlint-disable MD034 -->
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-previously-reviewed-and-published-application-to-the-teams-app-catalog"></a>Exemplo 2: atualizar um aplicativo previamente revisado e publicado para o catálogo de aplicativos do teams

### <a name="request"></a>Solicitação

<!-- markdownlint-disable MD034 -->
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

### <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `201 Created` código de resposta e o par de chave/valor `publishingState` : `submitted` no corpo da resposta. Para obter detalhes, consulte [teamsAppDefinition](../resources/teamsappdefinition.md).

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==

{
    "@odata.context": "https://graph.microsoft.com/v1/$metadata#appDefinition",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-08-08 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
