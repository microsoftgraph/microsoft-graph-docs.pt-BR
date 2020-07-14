---
title: Excluir profileCardProperty
description: Exclua um objeto profileCardProperty e remova todas as personalizações do cartão de perfil.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 64e3e26f37b9df3921a8bcd37eb27edd297b1998
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123965"
---
# <a name="delete-profilecardproperty"></a><span data-ttu-id="0d55f-103">Excluir profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="0d55f-103">Delete profileCardProperty</span></span>

<span data-ttu-id="0d55f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d55f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d55f-105">Exclua o objeto [profileCardProperty](../resources/profilecardproperty.md) especificado por seu `directoryPropertyName` do cartão de perfil da organização e remova quaisquer personalizações localizadas para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d55f-105">Delete the [profileCardProperty](../resources/profilecardproperty.md) object specified by its `directoryPropertyName` from the organization's profile card, and remove any localized customizations for that property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d55f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0d55f-106">Permissions</span></span>

<span data-ttu-id="0d55f-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0d55f-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0d55f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d55f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0d55f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0d55f-109">Permission type</span></span>                        | <span data-ttu-id="0d55f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0d55f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0d55f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0d55f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0d55f-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0d55f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="0d55f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0d55f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d55f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d55f-114">Not supported.</span></span>                              |
| <span data-ttu-id="0d55f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0d55f-115">Application</span></span>                            | <span data-ttu-id="0d55f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0d55f-116">Not supported.</span></span>                              |

><span data-ttu-id="0d55f-117">**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.</span><span class="sxs-lookup"><span data-stu-id="0d55f-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="0d55f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0d55f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{directoryPropertyName-Value}
```

## <a name="request-headers"></a><span data-ttu-id="0d55f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55f-119">Request headers</span></span>

| <span data-ttu-id="0d55f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="0d55f-120">Name</span></span>          | <span data-ttu-id="0d55f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d55f-121">Description</span></span>    |
|:--------------|:---------------|
| <span data-ttu-id="0d55f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0d55f-122">Authorization</span></span> | <span data-ttu-id="0d55f-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="0d55f-123">Bearer {token}.</span></span> <span data-ttu-id="0d55f-124">Required.</span><span class="sxs-lookup"><span data-stu-id="0d55f-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d55f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55f-125">Request body</span></span>

<span data-ttu-id="0d55f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0d55f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d55f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d55f-127">Response</span></span>

<span data-ttu-id="0d55f-128">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="0d55f-128">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="0d55f-129">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="0d55f-129">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d55f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0d55f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d55f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0d55f-131">Request</span></span>

<span data-ttu-id="0d55f-132">O exemplo a seguir mostra como excluir o atributo chamado "fax" do cartão de perfil da organização.</span><span class="sxs-lookup"><span data-stu-id="0d55f-132">The following example shows how to delete the attribute named "Fax" from the profile card for the organization.</span></span>

# <a name="http"></a>[<span data-ttu-id="0d55f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0d55f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_profilecardproperty"
}-->

```http
DELETE https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/fax
```
# <a name="c"></a>[<span data-ttu-id="0d55f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0d55f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0d55f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0d55f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0d55f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0d55f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0d55f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0d55f-137">Response</span></span>

<span data-ttu-id="0d55f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0d55f-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete profileCardProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
