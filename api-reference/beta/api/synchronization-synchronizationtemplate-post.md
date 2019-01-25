---
title: Criar synchronizationTemplate
description: Crie um novo modelo de sincronização para um determinado aplicativo.
localization_priority: Normal
ms.openlocfilehash: ce519b57766956b10d05b6b3745ca16f609b597c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509886"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="c532a-103">Criar synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c532a-103">Create synchronizationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c532a-104">Crie um novo modelo de sincronização para um determinado aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c532a-104">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c532a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c532a-105">Permissions</span></span>
<span data-ttu-id="c532a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c532a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c532a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c532a-108">Permission type</span></span>                        | <span data-ttu-id="c532a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c532a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c532a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c532a-110">Delegated (work or school account)</span></span>     |<span data-ttu-id="c532a-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c532a-111">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="c532a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c532a-112">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="c532a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c532a-113">Not supported.</span></span>|
|<span data-ttu-id="c532a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c532a-114">Application</span></span>                            |<span data-ttu-id="c532a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c532a-115">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="c532a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c532a-116">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="c532a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c532a-117">Request headers</span></span>

| <span data-ttu-id="c532a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="c532a-118">Name</span></span>           | <span data-ttu-id="c532a-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="c532a-119">Type</span></span>    | <span data-ttu-id="c532a-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="c532a-120">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="c532a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c532a-121">Authorization</span></span>  | <span data-ttu-id="c532a-122">string</span><span class="sxs-lookup"><span data-stu-id="c532a-122">string</span></span>  | <span data-ttu-id="c532a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c532a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c532a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c532a-125">Request body</span></span>

<span data-ttu-id="c532a-126">No corpo da solicitação, fornece o objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c532a-126">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="c532a-127">O `id`, `applicationId` e `factoryTag` propriedades são necessárias.</span><span class="sxs-lookup"><span data-stu-id="c532a-127">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="c532a-128">Quando não `schema` é fornecida com o modelo, o esquema padrão associado a `factoryTag` propriedade será usada.</span><span class="sxs-lookup"><span data-stu-id="c532a-128">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="c532a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c532a-129">Response</span></span>

<span data-ttu-id="c532a-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c532a-130">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="c532a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c532a-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c532a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c532a-132">Request</span></span>
<span data-ttu-id="c532a-133">O exemplo a seguir é um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c532a-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```

##### <a name="response"></a><span data-ttu-id="c532a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="c532a-134">Response</span></span>
<span data-ttu-id="c532a-135">O exemplo a seguir é um exemplo de uma resposta.</span><span class="sxs-lookup"><span data-stu-id="c532a-135">The following is an example of a response.</span></span>
><span data-ttu-id="c532a-136">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c532a-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c532a-137">Serão retornadas todas as propriedades em uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c532a-137">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/synchronization-synchronizationtemplate-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
