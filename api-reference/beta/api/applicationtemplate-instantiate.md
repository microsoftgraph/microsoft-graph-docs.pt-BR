---
title: 'applicationtemplate: instanciar'
description: Use esta API para criar um novo aplicativo
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f37cc7351449fc2fadbf259dde16682545ccc235
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441379"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="3b415-103">applicationtemplate: instanciar</span><span class="sxs-lookup"><span data-stu-id="3b415-103">applicationTemplate: instantiate</span></span>

<span data-ttu-id="3b415-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b415-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b415-105">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="3b415-105">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b415-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3b415-106">Permissions</span></span>

<span data-ttu-id="3b415-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b415-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3b415-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b415-109">Permission type</span></span>                        | <span data-ttu-id="3b415-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b415-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3b415-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b415-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3b415-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b415-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3b415-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b415-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b415-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b415-114">Not supported.</span></span> |
| <span data-ttu-id="3b415-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b415-115">Application</span></span>                            | <span data-ttu-id="3b415-116">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b415-116">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b415-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b415-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="3b415-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b415-118">Request headers</span></span>

| <span data-ttu-id="3b415-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3b415-119">Name</span></span>          | <span data-ttu-id="3b415-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b415-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3b415-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b415-121">Authorization</span></span> | <span data-ttu-id="3b415-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3b415-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b415-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b415-123">Request body</span></span>

<span data-ttu-id="3b415-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b415-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3b415-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3b415-125">Parameter</span></span>    | <span data-ttu-id="3b415-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b415-126">Type</span></span>        | <span data-ttu-id="3b415-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b415-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b415-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3b415-128">displayName</span></span>|<span data-ttu-id="3b415-129">String</span><span class="sxs-lookup"><span data-stu-id="3b415-129">String</span></span>|<span data-ttu-id="3b415-130">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b415-130">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="3b415-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b415-131">Response</span></span>

<span data-ttu-id="3b415-132">Se tiver êxito, este método retornará `201 OK` um código de resposta e um novo objeto [applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b415-132">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3b415-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3b415-133">Examples</span></span>

<span data-ttu-id="3b415-134">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3b415-134">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3b415-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b415-135">Request</span></span>

<span data-ttu-id="3b415-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b415-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3b415-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="3b415-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="3b415-138">C#</span><span class="sxs-lookup"><span data-stu-id="3b415-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3b415-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b415-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3b415-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3b415-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b415-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b415-141">Response</span></span>

<span data-ttu-id="3b415-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3b415-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="3b415-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3b415-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3b415-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b415-144">All the properties will be returned from an actual call.</span></span>

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
