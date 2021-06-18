---
title: Obter educationAssignmentSettings
description: Leia as propriedades e as relações de um objeto educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0c2758258126203ff8099dc5a162ade00a32ffb4
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993506"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="3c206-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="3c206-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="3c206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c206-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c206-105">Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3c206-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c206-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3c206-106">Permissions</span></span>
<span data-ttu-id="3c206-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c206-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c206-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3c206-109">Permission type</span></span>|<span data-ttu-id="3c206-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3c206-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c206-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3c206-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3c206-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c206-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="3c206-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3c206-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c206-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3c206-114">Not supported.</span></span>|
|<span data-ttu-id="3c206-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3c206-115">Application</span></span>| <span data-ttu-id="3c206-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3c206-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c206-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3c206-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3c206-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3c206-118">Optional query parameters</span></span>
<span data-ttu-id="3c206-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3c206-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3c206-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3c206-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c206-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3c206-121">Request headers</span></span>
|<span data-ttu-id="3c206-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3c206-122">Name</span></span>|<span data-ttu-id="3c206-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c206-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3c206-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3c206-124">Authorization</span></span>|<span data-ttu-id="3c206-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3c206-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c206-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3c206-127">Request body</span></span>
<span data-ttu-id="3c206-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="3c206-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c206-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c206-129">Response</span></span>

<span data-ttu-id="3c206-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3c206-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3c206-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3c206-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3c206-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3c206-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3c206-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c206-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="3c206-134">C#</span><span class="sxs-lookup"><span data-stu-id="3c206-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3c206-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c206-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3c206-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c206-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3c206-137">Java</span><span class="sxs-lookup"><span data-stu-id="3c206-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3c206-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3c206-138">Response</span></span>
<span data-ttu-id="3c206-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3c206-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

