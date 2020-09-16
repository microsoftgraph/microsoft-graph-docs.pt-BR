---
title: Atualizar teamsApp
description: 'Atualize um aplicativo publicado anteriormente em um catálogo de aplicativos do teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0dc3c5f3021c5479ef3eb6f227d7fbe512e0c122
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843160"
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
| Delegado (conta corporativa ou de estudante)     | AppCatalog. ReadWrite. All, Directory. ReadWrite. All |
| Delegado (conta corporativa ou de estudante) | AppCatalog.Submit|
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

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
