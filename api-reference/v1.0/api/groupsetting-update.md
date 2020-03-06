---
title: Atualizar uma configuração de grupo
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d7690c0db76c7087ff747397eb48e6f014720fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516812"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="ee545-103">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="ee545-103">Update a group setting</span></span>

<span data-ttu-id="ee545-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee545-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee545-105">Atualize as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="ee545-105">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee545-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ee545-106">Permissions</span></span>

<span data-ttu-id="ee545-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee545-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ee545-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ee545-109">Permission type</span></span>      | <span data-ttu-id="ee545-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ee545-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee545-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee545-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee545-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ee545-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ee545-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee545-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee545-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee545-114">Not supported.</span></span>    |
|<span data-ttu-id="ee545-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee545-115">Application</span></span> | <span data-ttu-id="ee545-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee545-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee545-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee545-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ee545-118">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="ee545-118">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ee545-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee545-119">Request headers</span></span>
| <span data-ttu-id="ee545-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ee545-120">Name</span></span> | <span data-ttu-id="ee545-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee545-121">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="ee545-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee545-122">Authorization</span></span>  | <span data-ttu-id="ee545-123">{token}.</span><span class="sxs-lookup"><span data-stu-id="ee545-123">{token}.</span></span> <span data-ttu-id="ee545-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee545-124">Required.</span></span> |
| <span data-ttu-id="ee545-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ee545-125">Content-Type</span></span>  | <span data-ttu-id="ee545-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee545-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ee545-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee545-127">Request body</span></span>
<span data-ttu-id="ee545-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="ee545-128">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="ee545-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee545-129">Property</span></span> | <span data-ttu-id="ee545-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee545-130">Type</span></span> | <span data-ttu-id="ee545-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee545-131">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ee545-132">values</span><span class="sxs-lookup"><span data-stu-id="ee545-132">values</span></span> | <span data-ttu-id="ee545-133">coleção SettingValue</span><span class="sxs-lookup"><span data-stu-id="ee545-133">settingValue collection</span></span> | <span data-ttu-id="ee545-p103">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="ee545-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="ee545-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee545-137">Response</span></span>

<span data-ttu-id="ee545-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ee545-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee545-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee545-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ee545-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee545-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ee545-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee545-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "False"
    },
    {
      "name": "ClassificationDescriptions",
      "value": ""
    },
    {
      "name": "DefaultClassification",
      "value": ""
    },
    {
      "name": "PrefixSuffixNamingRequirement",
      "value": ""
    },
    {
      "name": "AllowGuestsToBeGroupOwner",
      "value": "False"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "True"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": "62e90394-69f5-4237-9190-012177145e10"
    },
    {
      "name": "AllowToAddGuests",
      "value": "True"
    },
    {
      "name": "UsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "ClassificationList",
      "value": ""
    },
    {
      "name": "EnableGroupCreation",
      "value": "True"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ee545-142">C#</span><span class="sxs-lookup"><span data-stu-id="ee545-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee545-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee545-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee545-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee545-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee545-145">Java</span><span class="sxs-lookup"><span data-stu-id="ee545-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ee545-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee545-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
