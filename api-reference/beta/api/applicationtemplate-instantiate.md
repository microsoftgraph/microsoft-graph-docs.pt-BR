---
title: 'applicationtemplate: instanciar'
description: Use esta API para criar um novo aplicativo
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d8ae72372332979c1d6acc3d9d06e8913b454d9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408178"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="08920-103">applicationtemplate: instanciar</span><span class="sxs-lookup"><span data-stu-id="08920-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08920-104">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="08920-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="08920-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="08920-105">Permissions</span></span>

<span data-ttu-id="08920-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08920-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08920-108">Permission type</span></span>                        | <span data-ttu-id="08920-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08920-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="08920-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08920-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="08920-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08920-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="08920-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08920-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08920-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08920-113">Not supported.</span></span> |
| <span data-ttu-id="08920-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08920-114">Application</span></span>                            | <span data-ttu-id="08920-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08920-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08920-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08920-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="08920-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08920-117">Request headers</span></span>

| <span data-ttu-id="08920-118">Nome</span><span class="sxs-lookup"><span data-stu-id="08920-118">Name</span></span>          | <span data-ttu-id="08920-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="08920-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="08920-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="08920-120">Authorization</span></span> | <span data-ttu-id="08920-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="08920-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="08920-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08920-122">Request body</span></span>

<span data-ttu-id="08920-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08920-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08920-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08920-124">Parameter</span></span>    | <span data-ttu-id="08920-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="08920-125">Type</span></span>        | <span data-ttu-id="08920-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="08920-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="08920-127">displayName</span><span class="sxs-lookup"><span data-stu-id="08920-127">displayName</span></span>|<span data-ttu-id="08920-128">String</span><span class="sxs-lookup"><span data-stu-id="08920-128">String</span></span>|<span data-ttu-id="08920-129">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="08920-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="08920-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="08920-130">Response</span></span>

<span data-ttu-id="08920-131">Se tiver êxito, este método retornará `201 OK` um código de resposta e um novo objeto [applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08920-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="08920-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="08920-132">Examples</span></span>

<span data-ttu-id="08920-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="08920-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="08920-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08920-134">Request</span></span>

<span data-ttu-id="08920-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08920-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08920-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="08920-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="08920-137">C#</span><span class="sxs-lookup"><span data-stu-id="08920-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08920-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08920-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08920-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08920-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="08920-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="08920-140">Response</span></span>

<span data-ttu-id="08920-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08920-141">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="08920-142">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="08920-142">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="08920-143">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08920-143">All the properties will be returned from an actual call.</span></span>

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
