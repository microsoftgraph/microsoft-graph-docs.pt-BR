---
title: Obter educationAssignmentSettings
description: Leia as propriedades e os relacionamentos de um objeto educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8a9d0be04c615c6affc7cf2bb0dfe4a4496e064b
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092523"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="d3a45-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d3a45-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="d3a45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3a45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3a45-105">Leia as propriedades e os relacionamentos de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d3a45-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3a45-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3a45-106">Permissions</span></span>
<span data-ttu-id="d3a45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3a45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3a45-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3a45-109">Permission type</span></span>|<span data-ttu-id="d3a45-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3a45-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3a45-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3a45-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3a45-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3a45-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="d3a45-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3a45-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3a45-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a45-114">Not supported.</span></span>|
|<span data-ttu-id="d3a45-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3a45-115">Application</span></span>|<span data-ttu-id="d3a45-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3a45-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3a45-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a45-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3a45-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d3a45-118">Optional query parameters</span></span>
<span data-ttu-id="d3a45-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a45-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d3a45-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d3a45-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3a45-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a45-121">Request headers</span></span>
|<span data-ttu-id="d3a45-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d3a45-122">Name</span></span>|<span data-ttu-id="d3a45-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3a45-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d3a45-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3a45-124">Authorization</span></span>|<span data-ttu-id="d3a45-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d3a45-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3a45-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a45-127">Request body</span></span>
<span data-ttu-id="d3a45-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d3a45-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3a45-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a45-129">Response</span></span>

<span data-ttu-id="d3a45-130">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3a45-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3a45-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3a45-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3a45-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3a45-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d3a45-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3a45-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="d3a45-134">C#</span><span class="sxs-lookup"><span data-stu-id="d3a45-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3a45-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3a45-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3a45-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3a45-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3a45-137">Java</span><span class="sxs-lookup"><span data-stu-id="d3a45-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3a45-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3a45-138">Response</span></span>
<span data-ttu-id="d3a45-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d3a45-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "submissionAnimationDisabled": false
  }
}
```

