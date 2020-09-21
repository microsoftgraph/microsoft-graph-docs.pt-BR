---
title: Criar uma configuração de grupo
description: Crie uma nova configuração, com base nos modelos disponíveis no groupSettingTemplates.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e75ec34b1049a761cdca6ab74b714a1aa75a7f22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973376"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="8d34d-103">Criar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="8d34d-103">Create a group setting</span></span>

<span data-ttu-id="8d34d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d34d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d34d-p101">Use essa API para criar uma nova configuração com base nos modelos disponíveis em [groupSettingTemplates](../resources/groupsettingtemplate.md). Essas configurações podem ser no nível do locatário ou do grupo. A solicitação de criação precisa fornecer [settingValues](../resources/settingvalue.md) para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que rege se os membros de um grupo podem convidar usuários convidados pode ser definida. Isso controlará esse comportamento depois que a capacidade de adicionar usuários convidados a um grupo esteja disponível de forma geral.</span><span class="sxs-lookup"><span data-stu-id="8d34d-p101">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="8d34d-110">Para obter uma lista de modelos e as propriedades que eles dão suporte no v 1.0, use uma [consulta groupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (para pontos de extremidade beta, Call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span><span class="sxs-lookup"><span data-stu-id="8d34d-110">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplates query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="8d34d-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="8d34d-111">Permissions</span></span>

<span data-ttu-id="8d34d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d34d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8d34d-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d34d-114">Permission type</span></span>      | <span data-ttu-id="8d34d-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8d34d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d34d-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d34d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8d34d-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d34d-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d34d-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d34d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d34d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d34d-119">Not supported.</span></span>    |
|<span data-ttu-id="8d34d-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d34d-120">Application</span></span> | <span data-ttu-id="8d34d-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d34d-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d34d-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d34d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="8d34d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d34d-123">Request headers</span></span>

| <span data-ttu-id="8d34d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="8d34d-124">Name</span></span> | <span data-ttu-id="8d34d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d34d-125">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="8d34d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d34d-126">Authorization</span></span> | <span data-ttu-id="8d34d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d34d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8d34d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8d34d-129">Content-Type</span></span> | <span data-ttu-id="8d34d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="8d34d-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d34d-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d34d-131">Request body</span></span>
<span data-ttu-id="8d34d-p104">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md). No entanto, o nome de exibição para que a configuração será definida com base no nome do modelo configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="8d34d-p104">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="8d34d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d34d-134">Response</span></span>

<span data-ttu-id="8d34d-135">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d34d-135">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d34d-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d34d-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8d34d-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d34d-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8d34d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d34d-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8d34d-139">C#</span><span class="sxs-lookup"><span data-stu-id="8d34d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-groupsetting-from-groupsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d34d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d34d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-groupsetting-from-groupsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d34d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d34d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-groupsetting-from-groupsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8d34d-142">Java</span><span class="sxs-lookup"><span data-stu-id="8d34d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-groupsetting-from-groupsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="8d34d-143">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).</span><span class="sxs-lookup"><span data-stu-id="8d34d-143">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8d34d-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d34d-144">Response</span></span>

<span data-ttu-id="8d34d-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d34d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

