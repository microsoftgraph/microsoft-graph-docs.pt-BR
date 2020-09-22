---
title: 'applicationtemplate: instanciar'
description: Use esta API para criar um novo aplicativo
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a06ace04fd87b91e56834fe874c8f6de141d7020
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996658"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="d3207-103">applicationtemplate: instanciar</span><span class="sxs-lookup"><span data-stu-id="d3207-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="d3207-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3207-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3207-105">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="d3207-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3207-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3207-106">Permissions</span></span>

<span data-ttu-id="d3207-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3207-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3207-109">Permission type</span></span>                        | <span data-ttu-id="d3207-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3207-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3207-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3207-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3207-112">Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d3207-112">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="d3207-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3207-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3207-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3207-114">Not supported.</span></span> |
| <span data-ttu-id="d3207-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3207-115">Application</span></span>                            | <span data-ttu-id="d3207-116">Application. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d3207-116">Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3207-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3207-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="d3207-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3207-118">Request headers</span></span>

| <span data-ttu-id="d3207-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3207-119">Name</span></span>          | <span data-ttu-id="d3207-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3207-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d3207-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3207-121">Authorization</span></span> | <span data-ttu-id="d3207-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d3207-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3207-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3207-123">Request body</span></span>

<span data-ttu-id="d3207-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3207-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3207-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d3207-125">Parameter</span></span>    | <span data-ttu-id="d3207-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3207-126">Type</span></span>        | <span data-ttu-id="d3207-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3207-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d3207-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d3207-128">displayName</span></span>|<span data-ttu-id="d3207-129">String</span><span class="sxs-lookup"><span data-stu-id="d3207-129">String</span></span>|<span data-ttu-id="d3207-130">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3207-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="d3207-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3207-131">Response</span></span>

<span data-ttu-id="d3207-132">Se tiver êxito, este método retornará um `201 OK` código de resposta e um novo objeto [applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3207-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3207-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3207-133">Examples</span></span>

<span data-ttu-id="d3207-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="d3207-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d3207-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3207-135">Request</span></span>

<span data-ttu-id="d3207-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3207-136">The following is an example of the request.</span></span>

> [!NOTE] 
> <span data-ttu-id="d3207-137">Você pode usar essa API para instanciar [aplicativos não-Galeria](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app).</span><span class="sxs-lookup"><span data-stu-id="d3207-137">You can use this API to instantiate [non-gallery apps](https://docs.microsoft.com/azure/active-directory/manage-apps/add-non-gallery-app).</span></span> <span data-ttu-id="d3207-138">Use a seguinte ID para **applicationtemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` .</span><span class="sxs-lookup"><span data-stu-id="d3207-138">Use the following ID for **applicationTemplate**: `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3207-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3207-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/beta/applicationTemplates/{id}/instantiate
Content-type: application/json

{
  "displayName": "My custom name"
}
```
# <a name="c"></a>[<span data-ttu-id="d3207-140">C#</span><span class="sxs-lookup"><span data-stu-id="d3207-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3207-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3207-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3207-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3207-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3207-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3207-143">Response</span></span>

<span data-ttu-id="d3207-144">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3207-144">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="d3207-145">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3207-145">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d3207-146">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3207-146">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json

{
   "servicePrincipal": {
      "accountEnabled": true,
      "addIns": [
        {
          "id": "id-value",
          "type": "type-value",
          "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
          ]
        }
      ],
      "appDisplayName": "appDisplayName-value",
      "appId": "appId-value",
      "appOwnerOrganizationId": "appOwnerOrganizationId-value",
      "appRoleAssignmentRequired": true
   },
   "application": {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


