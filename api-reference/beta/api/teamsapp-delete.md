---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aaf636772ed79e04d2e65a5d9243ea65a3d2b187
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990789"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a>Remover um aplicativo do catálogo de aplicativos da sua organização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). Para remover o aplicativo do catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .

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
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Nenhum.

>**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar. Não use a ID do manifesto do pacote de aplicativos zip.

## <a name="response"></a>Resposta

```
HTTP/1.1 204 No Content
```

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a>Resposta

```http
HTTP/1.1 204 No Content
```
