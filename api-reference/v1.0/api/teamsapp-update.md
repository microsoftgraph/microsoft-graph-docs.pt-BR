---
title: Permissions
description: 'Atualize um aplicativo publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 305711206200e7f515ecdb4caff290e8a5a27269
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814641"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a>Atualizar aplicativos publicados no catálogo de aplicativos da sua organização



Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino). Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Observação:** Somente os administradores globais podem chamar essa API.

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

Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

>**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar. Não use a ID do manifesto do pacote zip app.

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

Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)

### <a name="response"></a>Resposta

```
HTTP/1.1 204 No Content
```
