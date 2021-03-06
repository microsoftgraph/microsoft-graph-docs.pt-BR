---
title: Publicar teamsapp
description: 'Publique um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1984ed7226da71ba1baf1bf15a7d83df4e6609a0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471646"
---
# <a name="publish-teamsapp"></a>Publicar teamsapp

Namespace: microsoft.graph

Publique [um aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.
Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos de locatários); o recurso criado terá um **valor de propriedade distributionMethod** de `organization` .

A **propriedade requiresReview** permite que qualquer usuário envie um aplicativo para revisão por um administrador. Os administradores podem aprovar ou rejeitar esses aplicativos por meio dessa API ou do Centro de administração do Microsoft Teams.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegado (conta corporativa ou de estudante) | AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

Para publicar um aplicativo que exija uma revisão:

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a>Parâmetros de consulta

|Propriedade|Tipo|Descrição|
|----|----|----|
|requiresReview| Boolean | Esse parâmetro de consulta opcional aciona o processo de revisão do aplicativo. Os usuários com privilégios de administrador podem enviar aplicativos sem disparar uma revisão. Se os usuários quiserem solicitar uma revisão antes da publicação, eles deverão definir  `requiresReview` como `true` . Um usuário com privilégios de administrador pode optar por não definir ou definir o valor como e o aplicativo será considerado aprovado e `requiresReview` `false`  publicará instantaneamente.|

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | application/zip. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua uma carga de manifesto zip do Teams. Para obter detalhes, consulte [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).

Cada aplicativo no catálogo de aplicativos deve ter uma ID de manifesto exclusiva.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp.](../resources/teamsapp.md)

## <a name="examples"></a>Exemplos

### <a name="example-1-publish-an-app-to-the-app-catalog"></a>Exemplo 1: Publicar um aplicativo no catálogo de aplicativos

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

---
Para obter informações sobre como criar um arquivo zip de aplicativo do Microsoft Teams, consulte [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a>Exemplo 2: Carregar um novo aplicativo para revisão no catálogo de aplicativos de uma organização

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

---

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a>Exemplo 3: Aprovar ou rejeitar uma revisão pendente de um aplicativo

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortDescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```