---
title: Atualizar uma configuração de grupo
description: Atualize as propriedades de um objeto de configuração de grupo específico.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: a1b677e9d1a00dc01aaf2455ac075fe20cbe4d1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804953"
---
# <a name="update-a-group-setting"></a><span data-ttu-id="4d3fe-103">Atualizar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="4d3fe-103">Update a group setting</span></span>

<span data-ttu-id="4d3fe-104">Atualize as propriedades de um objeto de configuração de grupo específico.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-104">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d3fe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d3fe-105">Permissions</span></span>

<span data-ttu-id="4d3fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d3fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d3fe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d3fe-108">Permission type</span></span>      | <span data-ttu-id="4d3fe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d3fe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d3fe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d3fe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d3fe-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d3fe-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d3fe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d3fe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d3fe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-113">Not supported.</span></span>    |
|<span data-ttu-id="4d3fe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d3fe-114">Application</span></span> | <span data-ttu-id="4d3fe-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d3fe-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d3fe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d3fe-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="4d3fe-117">Atualizar uma configuração específica de grupo ou de locatário como um todo.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-117">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4d3fe-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="4d3fe-118">Optional request headers</span></span>
| <span data-ttu-id="4d3fe-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4d3fe-119">Name</span></span> | <span data-ttu-id="4d3fe-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d3fe-120">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="4d3fe-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d3fe-121">Authorization</span></span>  | <span data-ttu-id="4d3fe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d3fe-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d3fe-124">Content-Type</span></span>  | <span data-ttu-id="4d3fe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4d3fe-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d3fe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3fe-126">Request body</span></span>
<span data-ttu-id="4d3fe-127">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-127">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="4d3fe-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d3fe-128">Property</span></span> | <span data-ttu-id="4d3fe-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d3fe-129">Type</span></span> | <span data-ttu-id="4d3fe-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d3fe-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="4d3fe-131">values</span><span class="sxs-lookup"><span data-stu-id="4d3fe-131">values</span></span> | <span data-ttu-id="4d3fe-132">conjunto settingValue</span><span class="sxs-lookup"><span data-stu-id="4d3fe-132">settingValue collection</span></span> | <span data-ttu-id="4d3fe-p103">O conjunto atualizado de valores.  OBSERVAÇÃO: Você deve fornecer o conjunto inteiro. Você não pode atualizar um único conjunto de valores.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="4d3fe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3fe-136">Response</span></span>

<span data-ttu-id="4d3fe-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4d3fe-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4d3fe-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d3fe-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4d3fe-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d3fe-139">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="4d3fe-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d3fe-140">Response</span></span>

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
  "tocPath": ""
}-->
