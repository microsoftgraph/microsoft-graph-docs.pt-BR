---
title: Criar aplicativo
description: Use esta API para criar um novo aplicativo.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: b86030eede69b85d7b66e4ec5acdd7e2dfef0ce4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459105"
---
# <a name="create-application"></a><span data-ttu-id="f331f-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="f331f-103">Create Application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f331f-104">Use esta API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f331f-104">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="f331f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f331f-105">Permissions</span></span>
<span data-ttu-id="f331f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f331f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f331f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f331f-108">Permission type</span></span>      | <span data-ttu-id="f331f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f331f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f331f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f331f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f331f-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f331f-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f331f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f331f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f331f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f331f-113">Not supported.</span></span>    |
|<span data-ttu-id="f331f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f331f-114">Application</span></span> | <span data-ttu-id="f331f-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f331f-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f331f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f331f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="f331f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f331f-117">Request headers</span></span>
| <span data-ttu-id="f331f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f331f-118">Name</span></span>       | <span data-ttu-id="f331f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="f331f-119">Type</span></span> | <span data-ttu-id="f331f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f331f-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f331f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f331f-121">Authorization</span></span>  | <span data-ttu-id="f331f-122">string</span><span class="sxs-lookup"><span data-stu-id="f331f-122">string</span></span>  | <span data-ttu-id="f331f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f331f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f331f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f331f-125">Request body</span></span>
<span data-ttu-id="f331f-126">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f331f-126">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f331f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f331f-127">Response</span></span>

<span data-ttu-id="f331f-128">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [application](../resources/application.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f331f-128">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f331f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f331f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f331f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f331f-130">Request</span></span>
<span data-ttu-id="f331f-131">Eis um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f331f-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_applications"
}-->
```http
POST https://graph.microsoft.com/beta/applications
Content-type: application/json
Content-length: 67

{
  "allowPublicClient": true,
  "displayName": "Display name"
}
```
<span data-ttu-id="f331f-132">No corpo da solicitação, forneça uma representação JSON do objeto [application](../resources/application.md).</span><span class="sxs-lookup"><span data-stu-id="f331f-132">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f331f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f331f-133">Response</span></span>
<span data-ttu-id="f331f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f331f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 1145

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
    "id": "b5b2920e-a47c-43b7-91ef-25ae96fddddd",
    "deletedDateTime": null,
    "api": {
        "acceptedAccessTokenVersion": 2,
        "publishedPermissionScopes": []
    },
    "allowPublicClient": true,
    "applicationAliases": [],
    "appRoles": [],
    "createdDateTime": "2017-05-25T16:33:04.3646617Z",
    "installedClients": {
        "redirectUrls": []
    },
    "displayName": "Display name",
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "orgRestrictions": [],
    "passwordCredentials": [],
    "preAuthorizedApplications": [],
    "requiredResourceAccess": [],
    "tags": [],
    "web": {
        "redirectUrls": [],
        "logoutUrl": null,
        "oauth2AllowImplicitFlow": null
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-applications.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
