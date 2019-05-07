---
title: Criar uma configuração de grupo
description: Use essa API para criar uma nova configuração, com base nos modelos disponíveis no groupSettingTemplates. Essas configurações podem ser no nível do locatário ou no nível do grupo. A solicitação de criação deve fornecer settingValues para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que determina se os membros de um grupo podem convidar usuários convidados podem ser definidos. Isso irá controlar esse comportamento assim que a capacidade de adicionar usuários convidados a um grupo estiver disponível.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8c559455c1525727a9fb397e4578839c8b6356f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613140"
---
# <a name="create-a-group-setting"></a><span data-ttu-id="02ded-107">Criar uma configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="02ded-107">Create a group setting</span></span>

<span data-ttu-id="02ded-p102">Use essa API para criar uma nova configuração com base nos modelos disponíveis em [groupSettingTemplates](../resources/groupsettingtemplate.md). Essas configurações podem ser no nível do locatário ou do grupo. A solicitação de criação precisa fornecer [settingValues](../resources/settingvalue.md) para todas as configurações definidas no modelo. Para configurações específicas de grupo, somente a configuração que rege se os membros de um grupo podem convidar usuários convidados pode ser definida. Isso controlará esse comportamento depois que a capacidade de adicionar usuários convidados a um grupo esteja disponível de forma geral.</span><span class="sxs-lookup"><span data-stu-id="02ded-p102">Use this API to create a new setting, based on the templates available in [groupSettingTemplates](../resources/groupsettingtemplate.md). These settings can be at the tenant-level or at the group level. The creation request must provide [settingValues](../resources/settingvalue.md) for all the settings defined in the template. For group-specific settings, only the setting governing whether members of a group can invite guest users can be set. This will govern this behavior once the ability to add guest users to a group is generally available.</span></span>

<span data-ttu-id="02ded-113">Para obter uma lista de modelos e as propriedades que eles dão suporte no v 1.0, use uma [consulta groupSettingTemplate](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0) (para pontos de extremidade beta, Call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span><span class="sxs-lookup"><span data-stu-id="02ded-113">For a list of templates and the properties they support in v1.0, use a [groupSettingTemplate query](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)  (For beta endpoints, call [directorySettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta).)</span></span>

## <a name="permissions"></a><span data-ttu-id="02ded-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="02ded-114">Permissions</span></span>

<span data-ttu-id="02ded-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02ded-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="02ded-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02ded-117">Permission type</span></span>      | <span data-ttu-id="02ded-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02ded-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02ded-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02ded-119">Delegated (work or school account)</span></span> | <span data-ttu-id="02ded-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02ded-120">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02ded-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02ded-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02ded-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02ded-122">Not supported.</span></span>    |
|<span data-ttu-id="02ded-123">Application</span><span class="sxs-lookup"><span data-stu-id="02ded-123">Application</span></span> | <span data-ttu-id="02ded-124">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02ded-124">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02ded-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02ded-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupSettings
POST /groups/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="02ded-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02ded-126">Request headers</span></span>

| <span data-ttu-id="02ded-127">Nome</span><span class="sxs-lookup"><span data-stu-id="02ded-127">Name</span></span> | <span data-ttu-id="02ded-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="02ded-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="02ded-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="02ded-129">Authorization</span></span> | <span data-ttu-id="02ded-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02ded-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02ded-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02ded-132">Content-Type</span></span> | <span data-ttu-id="02ded-133">application/json</span><span class="sxs-lookup"><span data-stu-id="02ded-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="02ded-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02ded-134">Request body</span></span>
<span data-ttu-id="02ded-p105">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md). No entanto, o nome de exibição para que a configuração será definida com base no nome do modelo configurações referenciado.</span><span class="sxs-lookup"><span data-stu-id="02ded-p105">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object. However, the display name for the setting will be set based on the referenced settings template name.</span></span>

## <a name="response"></a><span data-ttu-id="02ded-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="02ded-137">Response</span></span>

<span data-ttu-id="02ded-138">Se bem-sucedido, este método retorna o código de resposta `201 Created` e um objeto [groupSetting](../resources/groupsetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02ded-138">If successful, this method returns `201 Created` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02ded-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02ded-139">Example</span></span>

##### <a name="request"></a><span data-ttu-id="02ded-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02ded-140">Request</span></span>

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
<span data-ttu-id="02ded-141">No corpo da solicitação, forneça uma representação JSON do objeto [groupSetting](../resources/groupsetting.md).</span><span class="sxs-lookup"><span data-stu-id="02ded-141">In the request body, supply a JSON representation of [groupSetting](../resources/groupsetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="02ded-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="02ded-142">Response</span></span>

<span data-ttu-id="02ded-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02ded-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="02ded-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="02ded-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="02ded-146">Basic</span><span class="sxs-lookup"><span data-stu-id="02ded-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02ded-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02ded-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_groupsetting_from_groupsettings-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupsetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/groupsetting-post-groupsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
