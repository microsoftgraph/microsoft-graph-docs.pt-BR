---
title: Criar uma configuração de diretório em grupos
description: Use essa API para criar uma nova configuração de diretório para o grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d6879bdd6793cd29ee166c43a60beee275b865db
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323203"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="71675-103">Criar uma configuração de diretório em grupos</span><span class="sxs-lookup"><span data-stu-id="71675-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71675-104">Use essa API para criar uma nova configuração de diretório para o grupo.</span><span class="sxs-lookup"><span data-stu-id="71675-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="71675-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="71675-105">Permissions</span></span>
<span data-ttu-id="71675-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71675-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71675-108">Permission type</span></span>      | <span data-ttu-id="71675-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71675-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71675-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71675-110">Delegated (work or school account)</span></span> | <span data-ttu-id="71675-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71675-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71675-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71675-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71675-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="71675-113">Not supported.</span></span>    |
|<span data-ttu-id="71675-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71675-114">Application</span></span> | <span data-ttu-id="71675-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71675-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71675-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71675-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="71675-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71675-117">Request headers</span></span>
| <span data-ttu-id="71675-118">Nome</span><span class="sxs-lookup"><span data-stu-id="71675-118">Name</span></span>       | <span data-ttu-id="71675-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="71675-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71675-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="71675-120">Authorization</span></span>  | <span data-ttu-id="71675-121"><token> de portador.</span><span class="sxs-lookup"><span data-stu-id="71675-121">Bearer <token>.</span></span> <span data-ttu-id="71675-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="71675-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="71675-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71675-123">Request body</span></span>
<span data-ttu-id="71675-124">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="71675-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71675-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="71675-125">Response</span></span>

<span data-ttu-id="71675-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71675-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71675-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71675-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71675-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71675-128">Request</span></span>
<span data-ttu-id="71675-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71675-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="71675-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="71675-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="71675-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71675-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="71675-132">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="71675-132">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71675-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="71675-133">Response</span></span>
<span data-ttu-id="71675-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71675-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
