---
title: Permissões
description: 'Publica um aplicativo para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
ms.openlocfilehash: 76750e385c8048c44d77064722d84c5765c2bcc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306150"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>Publicar aplicativos ao catálogo de aplicativos da sua organização



Publica um [aplicativo](../resources/teamsapp.md) para o catálogo de aplicativos do Microsoft Teams. Especificamente, essa API publica o aplicativo catálogo da sua organização (o catálogo de aplicativos do inquilino); o recurso criado terá `distributionMethod`  =  `organization`.

## <a name="permissions"></a>Permissões

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
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | aplicativo/zip |

## <a name="request-body"></a>Corpo da solicitação

Carga de manifesto de Zip equipes. Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). Não é possível criar um aplicativo para uma organização que tem a mesma ID de manifesto do aplicativo outra organização em questão.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Para obter informações sobre como criar um arquivo do Microsoft Teams aplicativo zip, consulte [criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). 

### <a name="response"></a>Resposta

```
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
