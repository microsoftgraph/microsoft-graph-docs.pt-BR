---
title: Atualizar o teamworkTag
description: Atualize as propriedades de um objeto teamworkTag.
author: anniecolonna
localization_priority: Normal
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 93e78b863c0b03f475c0d6e52a12316d4eee580d
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210100"
---
# <a name="update-teamworktag"></a><span data-ttu-id="67252-103">Atualizar o teamworkTag</span><span class="sxs-lookup"><span data-stu-id="67252-103">Update teamworkTag</span></span>
<span data-ttu-id="67252-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67252-105">Atualize as propriedades de um [objeto teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="67252-105">Update the properties of a [teamworkTag](../resources/teamworktag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="67252-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="67252-106">Permissions</span></span>
<span data-ttu-id="67252-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67252-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67252-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67252-109">Permission type</span></span>|<span data-ttu-id="67252-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="67252-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67252-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67252-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67252-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67252-112">Not supported.</span></span>|
|<span data-ttu-id="67252-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67252-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67252-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67252-114">Not supported.</span></span>|
|<span data-ttu-id="67252-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67252-115">Application</span></span>|<span data-ttu-id="67252-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67252-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67252-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67252-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /teams/{team-Id}/tags/{teamworkTag-Id}
```

## <a name="request-headers"></a><span data-ttu-id="67252-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67252-118">Request headers</span></span>
|<span data-ttu-id="67252-119">Nome</span><span class="sxs-lookup"><span data-stu-id="67252-119">Name</span></span>|<span data-ttu-id="67252-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="67252-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="67252-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="67252-121">Authorization</span></span>|<span data-ttu-id="67252-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67252-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67252-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67252-124">Content-Type</span></span>|<span data-ttu-id="67252-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67252-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67252-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67252-127">Request body</span></span>
<span data-ttu-id="67252-128">No corpo da solicitação, fornece uma representação JSON do [objeto teamworkTag.](../resources/teamworktag.md)</span><span class="sxs-lookup"><span data-stu-id="67252-128">In the request body, supply a JSON representation of the [teamworkTag](../resources/teamworktag.md) object.</span></span>

<span data-ttu-id="67252-129">A tabela a seguir mostra as propriedades que são necessárias ao atualizar o trabalho em [equipeTag](../resources/teamworktag.md).</span><span class="sxs-lookup"><span data-stu-id="67252-129">The following table shows the properties that are required when you update the [teamworkTag](../resources/teamworktag.md).</span></span>

|<span data-ttu-id="67252-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67252-130">Property</span></span>|<span data-ttu-id="67252-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67252-131">Type</span></span>|<span data-ttu-id="67252-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67252-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67252-133">displayName</span><span class="sxs-lookup"><span data-stu-id="67252-133">displayName</span></span>|<span data-ttu-id="67252-134">String</span><span class="sxs-lookup"><span data-stu-id="67252-134">String</span></span>|<span data-ttu-id="67252-135">Nome da marca.</span><span class="sxs-lookup"><span data-stu-id="67252-135">Name of the tag.</span></span> <span data-ttu-id="67252-136">O valor não pode ter mais de 40 caracteres.</span><span class="sxs-lookup"><span data-stu-id="67252-136">The value can't be more than 40 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="67252-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="67252-137">Response</span></span>

<span data-ttu-id="67252-138">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkTag](../resources/teamworktag.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67252-138">If successful, this method returns a `200 OK` response code and an updated [teamworkTag](../resources/teamworktag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="67252-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="67252-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="67252-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67252-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="67252-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="67252-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamworktag"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==
Content-Type: application/json
Content-length: 185

{
  "displayName": "Finance"
}
```
# <a name="c"></a>[<span data-ttu-id="67252-142">C#</span><span class="sxs-lookup"><span data-stu-id="67252-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamworktag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67252-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67252-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamworktag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67252-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67252-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-teamworktag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="67252-145">Java</span><span class="sxs-lookup"><span data-stu-id="67252-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-teamworktag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="67252-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="67252-146">Response</span></span>
><span data-ttu-id="67252-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="67252-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamworkTag",
  "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==",
  "teamId": "53c53217-fe77-4383-bc5a-ed4937a1aecd",
  "displayName": "Finance",
  "memberCount": 2,
  "tagType": "standard"
}
```
