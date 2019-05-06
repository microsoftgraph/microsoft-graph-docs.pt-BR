---
title: Criar uma configuração de diretório em grupos
description: Use essa API para criar uma nova configuração de diretório para o grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7663917e2433862dd4eddfb385214e71f42d1375
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33592486"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="1eb3b-103">Criar uma configuração de diretório em grupos</span><span class="sxs-lookup"><span data-stu-id="1eb3b-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1eb3b-104">Use essa API para criar uma nova configuração de diretório para o grupo.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="1eb3b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1eb3b-105">Permissions</span></span>
<span data-ttu-id="1eb3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb3b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb3b-108">Permission type</span></span>      | <span data-ttu-id="1eb3b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1eb3b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1eb3b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb3b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1eb3b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1eb3b-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1eb3b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb3b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1eb3b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-113">Not supported.</span></span>    |
|<span data-ttu-id="1eb3b-114">Application</span><span class="sxs-lookup"><span data-stu-id="1eb3b-114">Application</span></span> | <span data-ttu-id="1eb3b-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb3b-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1eb3b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb3b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="1eb3b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb3b-117">Request headers</span></span>
| <span data-ttu-id="1eb3b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="1eb3b-118">Name</span></span>       | <span data-ttu-id="1eb3b-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="1eb3b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1eb3b-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb3b-120">Authorization</span></span>  | <span data-ttu-id="1eb3b-121"><token> de portador.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-121">Bearer <token>.</span></span> <span data-ttu-id="1eb3b-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="1eb3b-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eb3b-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb3b-123">Request body</span></span>
<span data-ttu-id="1eb3b-124">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="1eb3b-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1eb3b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb3b-125">Response</span></span>

<span data-ttu-id="1eb3b-126">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eb3b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1eb3b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1eb3b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb3b-128">Request</span></span>
<span data-ttu-id="1eb3b-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="1eb3b-130">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="1eb3b-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1eb3b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb3b-131">Response</span></span>
<span data-ttu-id="1eb3b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1eb3b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1eb3b-135">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="1eb3b-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1eb3b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1eb3b-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directorysetting_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
