---
title: Criar trabalho em equipeTagMember
description: Crie um novo objeto teamworkTagMember.
author: anniecolonna
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9376b8ddb690d4aaee1d571c83e0d94b96482935
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210133"
---
# <a name="create-teamworktagmember"></a><span data-ttu-id="46377-103">Criar trabalho em equipeTagMember</span><span class="sxs-lookup"><span data-stu-id="46377-103">Create teamworkTagMember</span></span>
<span data-ttu-id="46377-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46377-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46377-105">Crie um novo [objeto teamworkTagMember](../resources/teamworktagmember.md) em uma equipe.</span><span class="sxs-lookup"><span data-stu-id="46377-105">Create a new [teamworkTagMember](../resources/teamworktagmember.md) object in a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="46377-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="46377-106">Permissions</span></span>
<span data-ttu-id="46377-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46377-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46377-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46377-109">Permission type</span></span>|<span data-ttu-id="46377-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46377-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46377-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46377-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46377-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46377-112">Not supported.</span></span>|
|<span data-ttu-id="46377-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46377-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46377-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46377-114">Not supported.</span></span>|
|<span data-ttu-id="46377-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46377-115">Application</span></span>|<span data-ttu-id="46377-116">TeamworkTag.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46377-116">TeamworkTag.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46377-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46377-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{team-Id}/tags/{teamworkTag-Id}/members
```

## <a name="request-headers"></a><span data-ttu-id="46377-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46377-118">Request headers</span></span>
|<span data-ttu-id="46377-119">Nome</span><span class="sxs-lookup"><span data-stu-id="46377-119">Name</span></span>|<span data-ttu-id="46377-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="46377-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46377-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="46377-121">Authorization</span></span>|<span data-ttu-id="46377-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46377-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="46377-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="46377-124">Content-Type</span></span>|<span data-ttu-id="46377-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46377-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46377-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46377-127">Request body</span></span>
<span data-ttu-id="46377-128">No corpo da solicitação, fornece uma representação JSON do [objeto teamworkTagMember.](../resources/teamworktagmember.md)</span><span class="sxs-lookup"><span data-stu-id="46377-128">In the request body, supply a JSON representation of the [teamworkTagMember](../resources/teamworktagmember.md) object.</span></span>

<span data-ttu-id="46377-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o trabalho em [equipeTagMember](../resources/teamworktagmember.md).</span><span class="sxs-lookup"><span data-stu-id="46377-129">The following table shows the properties that are required when you create the [teamworkTagMember](../resources/teamworktagmember.md).</span></span>

|<span data-ttu-id="46377-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46377-130">Property</span></span>|<span data-ttu-id="46377-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="46377-131">Type</span></span>|<span data-ttu-id="46377-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="46377-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46377-133">userId</span><span class="sxs-lookup"><span data-stu-id="46377-133">userId</span></span>|<span data-ttu-id="46377-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46377-134">String</span></span>|<span data-ttu-id="46377-135">Identificador de usuário do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="46377-135">User identifier of the member of the team.</span></span>|



## <a name="response"></a><span data-ttu-id="46377-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="46377-136">Response</span></span>

<span data-ttu-id="46377-137">Se tiver êxito, este método retornará um código de resposta e um `201 Created` objeto [teamworkTagMember](../resources/teamworktagmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46377-137">If successful, this method returns a `201 Created` response code and a [teamworkTagMember](../resources/teamworktagmember.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46377-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46377-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46377-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46377-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="46377-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="46377-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamworktagmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/53c53217-fe77-4383-bc5a-ed4937a1aecd/tags/MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyM3ZDg4M2Q4Yi1hMTc5LTRkZDctOTNiMy1hOGQzZGUxYTIxMmUjI3RhY29VSjN2RGk==/members
Content-Type: application/json
Content-length: 144

{
    "userId":"97f62344-57dc-409c-88ad-c4af14158ff5"
}
```
# <a name="c"></a>[<span data-ttu-id="46377-141">C#</span><span class="sxs-lookup"><span data-stu-id="46377-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-teamworktagmember-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="46377-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46377-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamworktagmember-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="46377-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46377-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamworktagmember-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="46377-144">Java</span><span class="sxs-lookup"><span data-stu-id="46377-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-teamworktagmember-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="46377-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="46377-145">Response</span></span>
><span data-ttu-id="46377-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="46377-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkTagMember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.teamworkTagMember",
    "id": "MjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyNlYjY1M2Y5Mi04MzczLTRkZTYtYmZlYy01YjRkMjE2YjZhZGUjI2QzYjJiM2ViLWM0N2YtNDViOS05NWYyLWIyZjJlZjYyMTVjZQ==",
    "displayName": "Megan Bowen",
    "tenantId": "18be64a9-c73a-4862-bccc-76c31ef09b9d",
    "userId": "92f6952f-61ca-4a94-8910-508a240bc167"
}
```

