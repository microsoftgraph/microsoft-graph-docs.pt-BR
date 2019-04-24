---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b89380a423bf01f6a2bd7e56086cc9290be094cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521828"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>Atualizar aplicativos publicados no catálogo de aplicativos da sua organização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams. Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). Para publicar no catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Observação:** Somente os administradores globais podem chamar esta API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegado (conta corporativa ou de estudante)     | AppCatalog.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | aplicativo/zip |

## <a name="request-body"></a>Corpo da solicitação

Carga do manifesto zip do teams: para o aplicativo do teams arquivo zip [consulte criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar. Não use a ID do manifesto do pacote de aplicativos zip.

## <a name="response"></a>Resposta

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Para o aplicativo do teams arquivo zip [consulte CREATE app Package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>Resposta

```
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
