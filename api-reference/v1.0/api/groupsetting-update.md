---
title: Atualizar uma configuração de grupo
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 5433504aec92d8fb96a00857ff4e27c7bfc200c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973397"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="172d2-103">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="172d2-103">Update a group setting</span></span>

<span data-ttu-id="172d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="172d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="172d2-105">Atualizar as propriedades de um objeto [groupSetting](../resources/groupsetting.md) para definições de [grupo](../resources/group.md) em todo o locatário ou uma configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="172d2-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="172d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="172d2-106">Permissions</span></span>

<span data-ttu-id="172d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="172d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="172d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="172d2-109">Permission type</span></span>      | <span data-ttu-id="172d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="172d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="172d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="172d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="172d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="172d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="172d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="172d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="172d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="172d2-114">Not supported.</span></span>    |
|<span data-ttu-id="172d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="172d2-115">Application</span></span> | <span data-ttu-id="172d2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="172d2-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="172d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="172d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="172d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="172d2-118">Request headers</span></span>
| <span data-ttu-id="172d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="172d2-119">Name</span></span> | <span data-ttu-id="172d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="172d2-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="172d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="172d2-121">Authorization</span></span>  | <span data-ttu-id="172d2-122">{token}.</span><span class="sxs-lookup"><span data-stu-id="172d2-122">{token}.</span></span> <span data-ttu-id="172d2-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="172d2-123">Required.</span></span> |
| <span data-ttu-id="172d2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="172d2-124">Content-Type</span></span>  | <span data-ttu-id="172d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="172d2-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="172d2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="172d2-126">Request body</span></span>
<span data-ttu-id="172d2-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="172d2-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="172d2-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="172d2-128">Property</span></span> | <span data-ttu-id="172d2-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="172d2-129">Type</span></span> | <span data-ttu-id="172d2-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="172d2-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="172d2-131">values</span><span class="sxs-lookup"><span data-stu-id="172d2-131">values</span></span> | <span data-ttu-id="172d2-132">coleção [SettingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="172d2-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="172d2-133">O conjunto de valores atualizado.</span><span class="sxs-lookup"><span data-stu-id="172d2-133">The updated set of values.</span></span> <span data-ttu-id="172d2-134">Você deve incluir todo o conjunto de coleta.</span><span class="sxs-lookup"><span data-stu-id="172d2-134">You must include the entire collection set.</span></span> <span data-ttu-id="172d2-135">Não é possível atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="172d2-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="172d2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="172d2-136">Response</span></span>

<span data-ttu-id="172d2-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="172d2-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="172d2-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="172d2-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="172d2-139">Exemplo 1: atualizar uma configuração de grupo em todo o locatário</span><span class="sxs-lookup"><span data-stu-id="172d2-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="172d2-140">Neste exemplo, `{id}` é o identificador do objeto groupSetting de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="172d2-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="172d2-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="172d2-141">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="172d2-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="172d2-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="172d2-143">C#</span><span class="sxs-lookup"><span data-stu-id="172d2-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tenant-setting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="172d2-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="172d2-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tenant-setting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="172d2-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="172d2-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tenant-setting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="172d2-146">Java</span><span class="sxs-lookup"><span data-stu-id="172d2-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tenant-setting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="172d2-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="172d2-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="172d2-148">Exemplo 2: atualizar uma configuração de grupo específico</span><span class="sxs-lookup"><span data-stu-id="172d2-148">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="172d2-149">Neste exemplo, o primeiro `{id}` na solicitação é o identificador do grupo e o segundo `{id}` é o identificador do objeto groupSetting.</span><span class="sxs-lookup"><span data-stu-id="172d2-149">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="172d2-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="172d2-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="172d2-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="172d2-151">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="172d2-152">C#</span><span class="sxs-lookup"><span data-stu-id="172d2-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-groupsetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="172d2-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="172d2-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-groupsetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="172d2-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="172d2-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-groupsetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="172d2-155">Java</span><span class="sxs-lookup"><span data-stu-id="172d2-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-groupsetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="172d2-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="172d2-156">Response</span></span>

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

