---
title: Atualizar uma configuração de grupo
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2a2a504aa8c736df33ef35d3bd131b6329fd499c
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679754"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="6df84-103">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="6df84-103">Update a group setting</span></span>

<span data-ttu-id="6df84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6df84-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6df84-105">Atualize as propriedades de um objeto [](../resources/group.md) [groupSetting](../resources/groupsetting.md) para configurações de grupo em todo o locatário ou uma configuração de grupo específica.</span><span class="sxs-lookup"><span data-stu-id="6df84-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="6df84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6df84-106">Permissions</span></span>

<span data-ttu-id="6df84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6df84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6df84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6df84-109">Permission type</span></span>      | <span data-ttu-id="6df84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6df84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6df84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6df84-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6df84-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6df84-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6df84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6df84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6df84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6df84-114">Not supported.</span></span>    |
|<span data-ttu-id="6df84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6df84-115">Application</span></span> | <span data-ttu-id="6df84-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6df84-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6df84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6df84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6df84-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6df84-118">Request headers</span></span>
| <span data-ttu-id="6df84-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6df84-119">Name</span></span> | <span data-ttu-id="6df84-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6df84-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="6df84-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6df84-121">Authorization</span></span>  | <span data-ttu-id="6df84-122">{token}.</span><span class="sxs-lookup"><span data-stu-id="6df84-122">{token}.</span></span> <span data-ttu-id="6df84-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6df84-123">Required.</span></span> |
| <span data-ttu-id="6df84-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6df84-124">Content-Type</span></span>  | <span data-ttu-id="6df84-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6df84-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6df84-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6df84-126">Request body</span></span>
<span data-ttu-id="6df84-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6df84-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="6df84-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6df84-128">Property</span></span> | <span data-ttu-id="6df84-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6df84-129">Type</span></span> | <span data-ttu-id="6df84-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6df84-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="6df84-131">values</span><span class="sxs-lookup"><span data-stu-id="6df84-131">values</span></span> | <span data-ttu-id="6df84-132">[coleção settingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6df84-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="6df84-133">O conjunto atualizado de valores.</span><span class="sxs-lookup"><span data-stu-id="6df84-133">The updated set of values.</span></span> <span data-ttu-id="6df84-134">Você deve incluir todo o conjunto de coleções.</span><span class="sxs-lookup"><span data-stu-id="6df84-134">You must include the entire collection set.</span></span> <span data-ttu-id="6df84-135">Não é possível atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="6df84-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="6df84-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6df84-136">Response</span></span>

<span data-ttu-id="6df84-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6df84-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6df84-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6df84-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="6df84-139">Exemplo 1: atualizar uma configuração de grupo em todo o locatário</span><span class="sxs-lookup"><span data-stu-id="6df84-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="6df84-140">Neste exemplo, é o identificador do objeto groupSetting em todo o `{id}` locatário.</span><span class="sxs-lookup"><span data-stu-id="6df84-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="6df84-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6df84-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6df84-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6df84-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tenant_setting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json

{
  "displayName": "Group.Unified",
  "templateId": "62375ab9-6b52-47ed-826b-58e47e0e304b",
  "values": [
    {
      "name": "EnableMIPLabels",
      "value": "false"
    },
    {
      "name": "CustomBlockedWordsList",
      "value": ""
    },
    {
      "name": "EnableMSStandardBlockedWords",
      "value": "false"
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
      "value": "false"
    },
    {
      "name": "AllowGuestsToAccessGroups",
      "value": "true"
    },
    {
      "name": "GuestUsageGuidelinesUrl",
      "value": ""
    },
    {
      "name": "GroupCreationAllowedGroupId",
      "value": ""
    },
    {
      "name": "AllowToAddGuests",
      "value": "true"
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
      "value": "true"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6df84-143">C#</span><span class="sxs-lookup"><span data-stu-id="6df84-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-setting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6df84-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6df84-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-setting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6df84-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6df84-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-setting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6df84-146">Java</span><span class="sxs-lookup"><span data-stu-id="6df84-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-setting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6df84-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6df84-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="6df84-148">Exemplo 2: Atualizar uma configuração de grupo específica</span><span class="sxs-lookup"><span data-stu-id="6df84-148">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="6df84-149">Neste exemplo, o primeiro na solicitação é o identificador do grupo e o segundo é o identificador do `{id}` `{id}` objeto groupSetting.</span><span class="sxs-lookup"><span data-stu-id="6df84-149">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="6df84-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6df84-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6df84-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="6df84-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/{id}/settings/{id}
Content-type: application/json

{
  "displayName": "GroupSettings",
  "templateId": "08d542b9-071f-4e16-94b0-74abb372e3d9",
  "values": [
    {
            "name": "AllowToAddGuests",
            "value": "false"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6df84-152">C#</span><span class="sxs-lookup"><span data-stu-id="6df84-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6df84-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6df84-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6df84-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6df84-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6df84-155">Java</span><span class="sxs-lookup"><span data-stu-id="6df84-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6df84-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="6df84-156">Response</span></span>

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

