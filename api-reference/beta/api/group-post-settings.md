---
title: Criar uma configuração de diretório em grupos
description: Use essa API para criar uma nova configuração de diretório para o grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8f4d7e70311d40b762bf5fc683ff9fd4c509ba82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418712"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="e49d2-103">Criar uma configuração de diretório em grupos</span><span class="sxs-lookup"><span data-stu-id="e49d2-103">Create a directory setting on groups</span></span>

<span data-ttu-id="e49d2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e49d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49d2-105">Use essa API para criar uma nova configuração de diretório para o grupo.</span><span class="sxs-lookup"><span data-stu-id="e49d2-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e49d2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e49d2-106">Permissions</span></span>
<span data-ttu-id="e49d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e49d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e49d2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e49d2-109">Permission type</span></span>      | <span data-ttu-id="e49d2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e49d2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e49d2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e49d2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e49d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e49d2-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e49d2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e49d2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e49d2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e49d2-114">Not supported.</span></span>    |
|<span data-ttu-id="e49d2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e49d2-115">Application</span></span> | <span data-ttu-id="e49d2-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e49d2-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e49d2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e49d2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="e49d2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e49d2-118">Request headers</span></span>
| <span data-ttu-id="e49d2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e49d2-119">Name</span></span>       | <span data-ttu-id="e49d2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e49d2-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e49d2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e49d2-121">Authorization</span></span>  | <span data-ttu-id="e49d2-122"><token> de portador.</span><span class="sxs-lookup"><span data-stu-id="e49d2-122">Bearer <token>.</span></span> <span data-ttu-id="e49d2-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e49d2-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49d2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e49d2-124">Request body</span></span>
<span data-ttu-id="e49d2-125">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="e49d2-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e49d2-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49d2-126">Response</span></span>

<span data-ttu-id="e49d2-127">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e49d2-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e49d2-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e49d2-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e49d2-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e49d2-129">Request</span></span>
<span data-ttu-id="e49d2-130">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e49d2-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e49d2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e49d2-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="e49d2-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e49d2-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e49d2-133">No corpo da solicitação, forneça uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="e49d2-133">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e49d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e49d2-134">Response</span></span>
<span data-ttu-id="e49d2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e49d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
