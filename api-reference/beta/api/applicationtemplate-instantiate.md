---
title: 'applicationtemplate: instanciar'
description: Use esta API para criar um novo aplicativo
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d3874f7e015816dbc76ce99fa1fc26f65727ad97
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147882"
---
# <a name="applicationtemplate-instantiate"></a><span data-ttu-id="8dbee-103">applicationtemplate: instanciar</span><span class="sxs-lookup"><span data-stu-id="8dbee-103">applicationTemplate: instantiate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dbee-104">Adicione uma instância de um aplicativo da Galeria de aplicativos do Azure AD ao seu diretório.</span><span class="sxs-lookup"><span data-stu-id="8dbee-104">Add an instance of an application from the Azure AD application gallery into your directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dbee-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8dbee-105">Permissions</span></span>

<span data-ttu-id="8dbee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8dbee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dbee-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8dbee-108">Permission type</span></span>                        | <span data-ttu-id="8dbee-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8dbee-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8dbee-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8dbee-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8dbee-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbee-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="8dbee-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8dbee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8dbee-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8dbee-113">Not supported.</span></span> |
| <span data-ttu-id="8dbee-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dbee-114">Application</span></span>                            | <span data-ttu-id="8dbee-115">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dbee-115">Application.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dbee-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8dbee-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{id}/instantiate
```

## <a name="request-headers"></a><span data-ttu-id="8dbee-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-117">Request headers</span></span>

| <span data-ttu-id="8dbee-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8dbee-118">Name</span></span>          | <span data-ttu-id="8dbee-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dbee-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8dbee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dbee-120">Authorization</span></span> | <span data-ttu-id="8dbee-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8dbee-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dbee-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-122">Request body</span></span>

<span data-ttu-id="8dbee-123">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dbee-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8dbee-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8dbee-124">Parameter</span></span>    | <span data-ttu-id="8dbee-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dbee-125">Type</span></span>        | <span data-ttu-id="8dbee-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dbee-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8dbee-127">displayName</span><span class="sxs-lookup"><span data-stu-id="8dbee-127">displayName</span></span>|<span data-ttu-id="8dbee-128">String</span><span class="sxs-lookup"><span data-stu-id="8dbee-128">String</span></span>|<span data-ttu-id="8dbee-129">Nome personalizado do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8dbee-129">Custom name of the application</span></span>|

## <a name="response"></a><span data-ttu-id="8dbee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbee-130">Response</span></span>

<span data-ttu-id="8dbee-131">Se tiver êxito, este método retornará `201 OK` um código de resposta e um novo objeto [applicationServicePrincipal](../resources/applicationserviceprincipal.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8dbee-131">If successful, this method returns a `201 OK` response code and a new [applicationServicePrincipal](../resources/applicationserviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dbee-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8dbee-132">Examples</span></span>

<span data-ttu-id="8dbee-133">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="8dbee-133">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="8dbee-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8dbee-134">Request</span></span>

<span data-ttu-id="8dbee-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8dbee-135">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8dbee-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8dbee-136">Response</span></span>

<span data-ttu-id="8dbee-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8dbee-137">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="8dbee-138">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8dbee-138">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8dbee-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8dbee-139">All the properties will be returned from an actual call.</span></span>

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
