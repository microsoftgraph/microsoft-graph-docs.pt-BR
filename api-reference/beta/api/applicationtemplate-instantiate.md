---
title: 'applicationtemplate: instanciar'
description: Use esta API para criar um novo aplicativo
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d754b0053cd63711f4c0a1ef35d8429be84883
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856684"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="87f40-103">applicationtemplate: instanciar</span><span class="sxs-lookup"><span data-stu-id="87f40-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87f40-104">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="87f40-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="87f40-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="87f40-105">Permissions</span></span>

<span data-ttu-id="87f40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87f40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="87f40-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87f40-108">Permission type</span></span>                        | <span data-ttu-id="87f40-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87f40-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="87f40-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87f40-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="87f40-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f40-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="87f40-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87f40-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87f40-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87f40-113">Not supported.</span></span> |
| <span data-ttu-id="87f40-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87f40-114">Application</span></span>                            | <span data-ttu-id="87f40-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f40-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f40-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87f40-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="87f40-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87f40-117">Request headers</span></span>

| <span data-ttu-id="87f40-118">Nome</span><span class="sxs-lookup"><span data-stu-id="87f40-118">Name</span></span>          | <span data-ttu-id="87f40-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="87f40-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="87f40-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="87f40-120">Authorization</span></span> | <span data-ttu-id="87f40-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="87f40-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="87f40-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87f40-122">Request body</span></span>

<span data-ttu-id="87f40-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87f40-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="87f40-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="87f40-124">Parameter</span></span>    | <span data-ttu-id="87f40-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="87f40-125">Type</span></span>        | <span data-ttu-id="87f40-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="87f40-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="87f40-127">displayName</span><span class="sxs-lookup"><span data-stu-id="87f40-127">displayName</span></span>|<span data-ttu-id="87f40-128">String</span><span class="sxs-lookup"><span data-stu-id="87f40-128">String</span></span>|<span data-ttu-id="87f40-129">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="87f40-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="87f40-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f40-130">Response</span></span>

<span data-ttu-id="87f40-131">Se tiver êxito, este método retornará `201 OK` um código de resposta e um novo objeto [applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87f40-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="87f40-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="87f40-132">Examples</span></span>

<span data-ttu-id="87f40-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="87f40-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="87f40-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87f40-134">Request</span></span>

<span data-ttu-id="87f40-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87f40-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="87f40-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="87f40-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="87f40-137">C#</span><span class="sxs-lookup"><span data-stu-id="87f40-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="87f40-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="87f40-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="87f40-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="87f40-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="87f40-140">Java</span><span class="sxs-lookup"><span data-stu-id="87f40-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="87f40-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f40-141">Response</span></span>

<span data-ttu-id="87f40-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87f40-142">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="87f40-143">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="87f40-143">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="87f40-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87f40-144">All the properties will be returned from an actual call.</span></span>

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
