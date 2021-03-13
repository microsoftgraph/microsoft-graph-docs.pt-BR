---
title: Obter educationAssignmentSettings
description: Leia as propriedades e as relações de um objeto educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e65a154b17a1b7e1491908b03a5125bc69006fcd
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50773631"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="afd4b-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="afd4b-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="afd4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd4b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afd4b-105">Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="afd4b-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afd4b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="afd4b-106">Permissions</span></span>
<span data-ttu-id="afd4b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="afd4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afd4b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="afd4b-109">Permission type</span></span>|<span data-ttu-id="afd4b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="afd4b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afd4b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="afd4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="afd4b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="afd4b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="afd4b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="afd4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afd4b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afd4b-114">Not supported.</span></span>|
|<span data-ttu-id="afd4b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="afd4b-115">Application</span></span>|<span data-ttu-id="afd4b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="afd4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afd4b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="afd4b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="afd4b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="afd4b-118">Optional query parameters</span></span>
<span data-ttu-id="afd4b-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="afd4b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="afd4b-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="afd4b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="afd4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4b-121">Request headers</span></span>
|<span data-ttu-id="afd4b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="afd4b-122">Name</span></span>|<span data-ttu-id="afd4b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="afd4b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="afd4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="afd4b-124">Authorization</span></span>|<span data-ttu-id="afd4b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afd4b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afd4b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4b-127">Request body</span></span>
<span data-ttu-id="afd4b-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="afd4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="afd4b-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="afd4b-129">Response</span></span>

<span data-ttu-id="afd4b-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="afd4b-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="afd4b-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="afd4b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="afd4b-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="afd4b-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="afd4b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="afd4b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="afd4b-134">C#</span><span class="sxs-lookup"><span data-stu-id="afd4b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afd4b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afd4b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afd4b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afd4b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="afd4b-137">Java</span><span class="sxs-lookup"><span data-stu-id="afd4b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afd4b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="afd4b-138">Response</span></span>
<span data-ttu-id="afd4b-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="afd4b-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

