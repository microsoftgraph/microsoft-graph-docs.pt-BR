---
title: Permissões
description: 'Publicar um aplicativo no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3560faff90e02da77e7a3a5a55dba4ce1ecf87d9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335294"
---
# <a name="publish-apps-to-your-organizations-app-catalog"></a>Publicar aplicativos no catálogo de aplicativos da sua organização

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Publicar um [aplicativo](../resources/teamsapp.md) no catálogo de aplicativos do Microsoft Teams. Especificamente, essa API publica o aplicativo no catálogo da sua organização (o catálogo de aplicativos do locatário); o recurso `distributionMethod`  =  `organization`criado terá.

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
POST /appCatalogs/teamsApps
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |
| Content-Type  | aplicativo/zip |

## <a name="request-body"></a>Corpo da solicitação

Carga do manifesto zip do teams. Para o arquivo zip do aplicativo do Teams, [consulte criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). Você não pode criar um aplicativo para uma organização que tenha a mesma ID de manifesto que outro aplicativo da organização.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

Para obter informações sobre como criar um arquivo zip do aplicativo do Microsoft Teams, consulte [criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package). 

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
