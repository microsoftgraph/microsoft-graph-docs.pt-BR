---
title: Atualizar uma configuração de grupo
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 29a83493884ffab11b10e8d48f051a45be1f1364
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892612"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="6a9db-103">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="6a9db-103">Update a group setting</span></span>

<span data-ttu-id="6a9db-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a9db-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a9db-105">Atualizar as propriedades de um objeto [groupSetting](../resources/groupsetting.md) para definições de [grupo](../resources/group.md) em todo o locatário ou uma configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="6a9db-105">Update the properties of a [groupSetting](../resources/groupsetting.md) object for tenant-wide [group](../resources/group.md) settings or a specific group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a9db-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6a9db-106">Permissions</span></span>

<span data-ttu-id="6a9db-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a9db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6a9db-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a9db-109">Permission type</span></span>      | <span data-ttu-id="6a9db-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6a9db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a9db-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a9db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6a9db-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a9db-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a9db-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a9db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a9db-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a9db-114">Not supported.</span></span>    |
|<span data-ttu-id="6a9db-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a9db-115">Application</span></span> | <span data-ttu-id="6a9db-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a9db-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a9db-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a9db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->



```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6a9db-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9db-118">Request headers</span></span>
| <span data-ttu-id="6a9db-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6a9db-119">Name</span></span> | <span data-ttu-id="6a9db-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9db-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="6a9db-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a9db-121">Authorization</span></span>  | <span data-ttu-id="6a9db-122">{token}.</span><span class="sxs-lookup"><span data-stu-id="6a9db-122">{token}.</span></span> <span data-ttu-id="6a9db-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a9db-123">Required.</span></span> |
| <span data-ttu-id="6a9db-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a9db-124">Content-Type</span></span>  | <span data-ttu-id="6a9db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a9db-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a9db-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9db-126">Request body</span></span>
<span data-ttu-id="6a9db-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="6a9db-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="6a9db-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a9db-128">Property</span></span> | <span data-ttu-id="6a9db-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a9db-129">Type</span></span> | <span data-ttu-id="6a9db-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a9db-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="6a9db-131">values</span><span class="sxs-lookup"><span data-stu-id="6a9db-131">values</span></span> | <span data-ttu-id="6a9db-132">coleção [SettingValue](../resources/settingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="6a9db-132">[settingValue](../resources/settingvalue.md) collection</span></span> | <span data-ttu-id="6a9db-133">O conjunto de valores atualizado.</span><span class="sxs-lookup"><span data-stu-id="6a9db-133">The updated set of values.</span></span> <span data-ttu-id="6a9db-134">Você deve incluir todo o conjunto de coleta.</span><span class="sxs-lookup"><span data-stu-id="6a9db-134">You must include the entire collection set.</span></span> <span data-ttu-id="6a9db-135">Não é possível atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="6a9db-135">You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="6a9db-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9db-136">Response</span></span>

<span data-ttu-id="6a9db-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6a9db-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6a9db-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6a9db-138">Examples</span></span>

### <a name="example-1-update-a-tenant-wide-group-setting"></a><span data-ttu-id="6a9db-139">Exemplo 1: atualizar uma configuração de grupo em todo o locatário</span><span class="sxs-lookup"><span data-stu-id="6a9db-139">Example 1: Update a tenant-wide group setting</span></span>

<span data-ttu-id="6a9db-140">Neste exemplo, `{id}` é o identificador do objeto groupSetting de todo o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a9db-140">In this example, `{id}` is the identifier of the tenant-wide groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="6a9db-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9db-141">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="6a9db-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9db-142">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-a-specific-group-setting"></a><span data-ttu-id="6a9db-143">Exemplo 2: atualizar uma configuração de grupo específico</span><span class="sxs-lookup"><span data-stu-id="6a9db-143">Example 2: Update a specific group setting</span></span>

<span data-ttu-id="6a9db-144">Neste exemplo, o primeiro `{id}` na solicitação é o identificador do grupo e o segundo `{id}` é o identificador do objeto groupSetting.</span><span class="sxs-lookup"><span data-stu-id="6a9db-144">In this example, the first `{id}` in the request is the identifier of the group, and the second `{id}` is the identifier of the groupSetting object.</span></span>

#### <a name="request"></a><span data-ttu-id="6a9db-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a9db-145">Request</span></span>

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

#### <a name="response"></a><span data-ttu-id="6a9db-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a9db-146">Response</span></span>

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
