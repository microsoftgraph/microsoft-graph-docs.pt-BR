---
title: Publicar teamsapp
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6aeef8c0faf1ab89b48d086839688e9ebe120efd
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843167"
---
# <a name="publish-teamsapp"></a>Publicar teamsapp

Namespace: microsoft.graph

Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams.
Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso criado terá um valor de propriedade **distributionMethod** de `organization` .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Observação:** Somente os administradores globais podem chamar esta API.

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegado (conta corporativa ou de estudante)     | AppCatalog. ReadWrite. All, Directory. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | Application/zip. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, inclua uma carga de manifesto zip do teams. Para obter detalhes, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).

Cada aplicativo no catálogo de aplicativos deve ter uma ID de manifesto exclusiva.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsApp](../resources/teamsapp.md) .

## <a name="examples"></a>Exemplos

### <a name="example-1-publish-an-app-to-the-app-catalog"></a>Exemplo 1: publicar um aplicativo no catálogo de aplicativos

#### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package).

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
