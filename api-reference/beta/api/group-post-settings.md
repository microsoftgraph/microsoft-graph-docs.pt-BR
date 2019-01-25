---
title: Criar uma configuração de diretório em grupos
description: Use essa API para criar uma nova configuração de diretório para o grupo.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 3ba33de148e34ce80c0a709a6a1b5faf99d5f32d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515843"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="545c2-103">Criar uma configuração de diretório em grupos</span><span class="sxs-lookup"><span data-stu-id="545c2-103">Create a directory setting on groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="545c2-104">Use essa API para criar uma nova configuração de diretório para o grupo.</span><span class="sxs-lookup"><span data-stu-id="545c2-104">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="545c2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="545c2-105">Permissions</span></span>
<span data-ttu-id="545c2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="545c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="545c2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="545c2-108">Permission type</span></span>      | <span data-ttu-id="545c2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="545c2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="545c2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="545c2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="545c2-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="545c2-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="545c2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="545c2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="545c2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="545c2-113">Not supported.</span></span>    |
|<span data-ttu-id="545c2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="545c2-114">Application</span></span> | <span data-ttu-id="545c2-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="545c2-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="545c2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="545c2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="545c2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="545c2-117">Request headers</span></span>
| <span data-ttu-id="545c2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="545c2-118">Name</span></span>       | <span data-ttu-id="545c2-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="545c2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="545c2-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="545c2-120">Authorization</span></span>  | <span data-ttu-id="545c2-121">Portador <token>.</span><span class="sxs-lookup"><span data-stu-id="545c2-121">Bearer <token>.</span></span> <span data-ttu-id="545c2-122">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="545c2-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="545c2-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="545c2-123">Request body</span></span>
<span data-ttu-id="545c2-124">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="545c2-124">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="545c2-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="545c2-125">Response</span></span>

<span data-ttu-id="545c2-126">Se tiver êxito, este método retornará `201 Created` objeto response de código e [directorySetting](../resources/directorysetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="545c2-126">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="545c2-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="545c2-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="545c2-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="545c2-128">Request</span></span>
<span data-ttu-id="545c2-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="545c2-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="545c2-130">No corpo da solicitação, fornece uma representação JSON do objeto [directorySetting](../resources/directorysetting.md) .</span><span class="sxs-lookup"><span data-stu-id="545c2-130">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="545c2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="545c2-131">Response</span></span>
<span data-ttu-id="545c2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="545c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/group-post-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
