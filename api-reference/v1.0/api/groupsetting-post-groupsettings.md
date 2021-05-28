---
title: Criar uma configuração de grupo
description: Crie uma nova configuração, com base nos modelos disponíveis em groupSettingTemplates.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4b3d67940a8d4ba71b3377c867edf2a0a8f11c80
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679761"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="ca68c-103">Criar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="ca68c-103">Create a group setting</span></span>

<span data-ttu-id="ca68c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca68c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ca68c-105">Use essa API para criar uma nova configuração, com base nos modelos disponíveis em [groupSettingTemplates](../resources/groupsettingtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="ca68c-105">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md).</span></span> <span data-ttu-id="ca68c-106">Essas configurações podem estar no nível do locatário ou no nível do grupo.</span><span class="sxs-lookup"><span data-stu-id="ca68c-106">These settings can be at the tenant-level or at the group level.</span></span> <span data-ttu-id="ca68c-107">A solicitação de criação deve [fornecer settingValues](../resources/settingvalue.md) para todas as configurações definidas no modelo.</span><span class="sxs-lookup"><span data-stu-id="ca68c-107">The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template.</span></span> <span data-ttu-id="ca68c-108">Para configurações específicas de grupo, somente a configuração que rege se membros de um grupo podem convidar usuários convidados podem ser definidos.</span><span class="sxs-lookup"><span data-stu-id="ca68c-108">For group-specific settings, only the setting governing whether members of a group can invite guest users can be set.</span></span> <span data-ttu-id="ca68c-109">Isso regerá esse comportamento quando a capacidade de adicionar usuários convidados a um grupo geralmente está disponível.</span><span class="sxs-lookup"><span data-stu-id="ca68c-109">This will govern this behavior once the ability to add guest users to a group is generally available.</span></span> <span data-ttu-id="ca68c-110">Para pontos de extremidade beta, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="ca68c-110">For beta endpoints, use [directorySettingTemplates](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="permissions"></a><span data-ttu-id="ca68c-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="ca68c-111">Permissions</span></span>

<span data-ttu-id="ca68c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca68c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ca68c-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca68c-114">Permission type</span></span>      | <span data-ttu-id="ca68c-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca68c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca68c-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca68c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="ca68c-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca68c-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca68c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca68c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca68c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca68c-119">Not supported.</span></span>    |
|<span data-ttu-id="ca68c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca68c-120">Application</span></span> | <span data-ttu-id="ca68c-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca68c-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca68c-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca68c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="ca68c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca68c-123">Request headers</span></span>

| <span data-ttu-id="ca68c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="ca68c-124">Name</span></span> | <span data-ttu-id="ca68c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca68c-125">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="ca68c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca68c-126">Authorization</span></span> | <span data-ttu-id="ca68c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca68c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ca68c-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ca68c-129">Content-Type</span></span> | <span data-ttu-id="ca68c-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ca68c-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca68c-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca68c-131">Request body</span></span>
<span data-ttu-id="ca68c-p104">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md). No entanto, o nome de exibição para que a configuração será definida com base no nome do modelo configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="ca68c-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="ca68c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca68c-134">Response</span></span>

<span data-ttu-id="ca68c-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca68c-135">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca68c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca68c-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ca68c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca68c-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ca68c-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca68c-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_groupsetting_from_groupsettings"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupSettings
Content-type: application/json
Content-length: 215

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ca68c-139">C#</span><span class="sxs-lookup"><span data-stu-id="ca68c-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca68c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca68c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca68c-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca68c-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ca68c-142">Java</span><span class="sxs-lookup"><span data-stu-id="ca68c-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="ca68c-143">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).</span><span class="sxs-lookup"><span data-stu-id="ca68c-143">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ca68c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca68c-144">Response</span></span>

<span data-ttu-id="ca68c-145">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ca68c-145">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 238

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ],
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

