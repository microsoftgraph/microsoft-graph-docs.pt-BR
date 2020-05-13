---
title: Lista atribuída tokenLifetimePolicies
description: Listar tokenLifetimePolicies atribuídos a um aplicativo ou a servicePrincipalName.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7c0523d501dd6b77bc5808b0f936f6692b12951b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43107231"
---
# <a name="list-assigned-tokenlifetimepolicy"></a><span data-ttu-id="dcf76-103">Lista atribuída tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="dcf76-103">List assigned tokenLifetimePolicy</span></span>

<span data-ttu-id="dcf76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcf76-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf76-105">Listar os objetos [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) que são atribuídos a um [aplicativo](../resources/application.md) ou [userdirigente](../resources/servicePrincipal.md)..</span><span class="sxs-lookup"><span data-stu-id="dcf76-105">List the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects that are assigned to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md)..</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf76-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcf76-106">Permissions</span></span>

<span data-ttu-id="dcf76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcf76-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcf76-109">Permission type</span></span>                        | <span data-ttu-id="dcf76-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcf76-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcf76-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcf76-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcf76-112">Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dcf76-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="dcf76-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcf76-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcf76-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcf76-114">Not supported.</span></span> |
| <span data-ttu-id="dcf76-115">Application</span><span class="sxs-lookup"><span data-stu-id="dcf76-115">Application</span></span>                            | <span data-ttu-id="dcf76-116">Policy. Read. All e Application. ReadWrite. OwnedBy, Policy. Read. All e Application. ReadWrite. All, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. OwnedBy, Policy. ReadWrite. ApplicationConfiguration e Application. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="dcf76-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcf76-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf76-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenLifetimePolicies
GET /servicePrincipals/{id}/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="dcf76-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf76-118">Request headers</span></span>

| <span data-ttu-id="dcf76-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dcf76-119">Name</span></span>          | <span data-ttu-id="dcf76-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf76-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dcf76-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcf76-121">Authorization</span></span> | <span data-ttu-id="dcf76-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="dcf76-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcf76-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf76-123">Request body</span></span>

<span data-ttu-id="dcf76-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcf76-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf76-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf76-125">Response</span></span>

<span data-ttu-id="dcf76-126">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf76-126">If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenLifetimePolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcf76-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcf76-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcf76-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf76-128">Request</span></span>

<span data-ttu-id="dcf76-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcf76-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcf76-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf76-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenlifetimepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
```
# <a name="c"></a>[<span data-ttu-id="dcf76-131">C#</span><span class="sxs-lookup"><span data-stu-id="dcf76-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenlifetimepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcf76-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcf76-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenlifetimepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcf76-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcf76-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenlifetimepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcf76-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf76-134">Response</span></span>

<span data-ttu-id="dcf76-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf76-135">The following is an example of the response.</span></span>

> <span data-ttu-id="dcf76-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcf76-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
