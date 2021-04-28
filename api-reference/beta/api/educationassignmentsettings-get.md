---
title: Obter educationAssignmentSettings
description: Leia as propriedades e as relações de um objeto educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f5f383ee9cfbb4824990b0c7c49da7852cbeb055
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061662"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="59983-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="59983-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="59983-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59983-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59983-105">Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="59983-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59983-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59983-106">Permissions</span></span>
<span data-ttu-id="59983-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59983-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59983-109">Permission type</span></span>|<span data-ttu-id="59983-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59983-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="59983-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59983-111">Delegated (work or school account)</span></span>|<span data-ttu-id="59983-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59983-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="59983-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59983-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59983-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59983-114">Not supported.</span></span>|
|<span data-ttu-id="59983-115">Application\*</span><span class="sxs-lookup"><span data-stu-id="59983-115">Application\*</span></span>| <span data-ttu-id="59983-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59983-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="59983-117">\*As permissões de aplicativo estão disponíveis apenas para clientes de visualização privada.</span><span class="sxs-lookup"><span data-stu-id="59983-117">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="59983-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59983-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59983-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59983-119">Optional query parameters</span></span>
<span data-ttu-id="59983-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59983-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="59983-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="59983-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="59983-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59983-122">Request headers</span></span>
|<span data-ttu-id="59983-123">Nome</span><span class="sxs-lookup"><span data-stu-id="59983-123">Name</span></span>|<span data-ttu-id="59983-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="59983-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="59983-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="59983-125">Authorization</span></span>|<span data-ttu-id="59983-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59983-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59983-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59983-128">Request body</span></span>
<span data-ttu-id="59983-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59983-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59983-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="59983-130">Response</span></span>

<span data-ttu-id="59983-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59983-131">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="59983-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="59983-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="59983-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59983-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="59983-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59983-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```
# <a name="c"></a>[<span data-ttu-id="59983-135">C#</span><span class="sxs-lookup"><span data-stu-id="59983-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59983-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59983-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59983-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59983-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59983-138">Java</span><span class="sxs-lookup"><span data-stu-id="59983-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="59983-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="59983-139">Response</span></span>
<span data-ttu-id="59983-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="59983-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

