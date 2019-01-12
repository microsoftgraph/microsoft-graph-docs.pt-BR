---
title: Criar aplicativo
description: Use essa API para criar um novo aplicativo.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 8cde90f31f7583d24361f6935701a91f69d7cfde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941468"
---
# <a name="create-application"></a><span data-ttu-id="fda81-103">Criar aplicativo</span><span class="sxs-lookup"><span data-stu-id="fda81-103">Create Application</span></span>

> <span data-ttu-id="fda81-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fda81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fda81-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fda81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fda81-106">Use essa API para criar um novo aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fda81-106">Use this API to create a new application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fda81-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="fda81-107">Permissions</span></span>
<span data-ttu-id="fda81-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fda81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fda81-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fda81-110">Permission type</span></span>      | <span data-ttu-id="fda81-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fda81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fda81-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fda81-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fda81-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fda81-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fda81-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fda81-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fda81-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fda81-115">Not supported.</span></span>    |
|<span data-ttu-id="fda81-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fda81-116">Application</span></span> | <span data-ttu-id="fda81-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda81-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fda81-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fda81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications
```

## <a name="request-headers"></a><span data-ttu-id="fda81-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fda81-119">Request headers</span></span>
| <span data-ttu-id="fda81-120">Nome</span><span class="sxs-lookup"><span data-stu-id="fda81-120">Name</span></span>       | <span data-ttu-id="fda81-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fda81-121">Type</span></span> | <span data-ttu-id="fda81-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda81-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fda81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fda81-123">Authorization</span></span>  | <span data-ttu-id="fda81-124">string</span><span class="sxs-lookup"><span data-stu-id="fda81-124">string</span></span>  | <span data-ttu-id="fda81-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fda81-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fda81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fda81-127">Request body</span></span>
<span data-ttu-id="fda81-128">No corpo da solicitação, fornece uma representação JSON do objeto [application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="fda81-128">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fda81-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="fda81-129">Response</span></span>

<span data-ttu-id="fda81-130">Se tiver êxito, este método retornará `201 Created` objeto de códigos e [aplicativos](../resources/application.md) de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fda81-130">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda81-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fda81-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fda81-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fda81-132">Request</span></span>
<span data-ttu-id="fda81-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fda81-133">Here is an example of the request.</span></span>
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
<span data-ttu-id="fda81-134">No corpo da solicitação, fornece uma representação JSON do objeto [application](../resources/application.md) .</span><span class="sxs-lookup"><span data-stu-id="fda81-134">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fda81-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="fda81-135">Response</span></span>
<span data-ttu-id="fda81-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fda81-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
