---
title: Obter educationAssignmentDefaults
description: Leia as propriedades e as relações de um objeto educationAssignmentDefaults.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 863ff034080250fc7ce4cfc5b22344fcd2374fad
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961293"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="5eb47-103">Obter educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="5eb47-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="5eb47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eb47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5eb47-105">Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="5eb47-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="5eb47-106">Esses são os padrões de atribuição de nível de classe respeitados pelas novas atribuições criadas na classe.</span><span class="sxs-lookup"><span data-stu-id="5eb47-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="5eb47-107">Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.</span><span class="sxs-lookup"><span data-stu-id="5eb47-107">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="5eb47-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="5eb47-108">Permissions</span></span>
<span data-ttu-id="5eb47-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5eb47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5eb47-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5eb47-111">Permission type</span></span>|<span data-ttu-id="5eb47-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5eb47-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5eb47-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5eb47-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5eb47-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eb47-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5eb47-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5eb47-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="5eb47-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5eb47-116">Not supported.</span></span> |
|<span data-ttu-id="5eb47-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5eb47-117">Application</span></span>| <span data-ttu-id="5eb47-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5eb47-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5eb47-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb47-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5eb47-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5eb47-120">Optional query parameters</span></span>
<span data-ttu-id="5eb47-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb47-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5eb47-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5eb47-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5eb47-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb47-123">Request headers</span></span>
|<span data-ttu-id="5eb47-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5eb47-124">Name</span></span>|<span data-ttu-id="5eb47-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5eb47-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5eb47-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5eb47-126">Authorization</span></span>|<span data-ttu-id="5eb47-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5eb47-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5eb47-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb47-129">Request body</span></span>
<span data-ttu-id="5eb47-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5eb47-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5eb47-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb47-131">Response</span></span>

<span data-ttu-id="5eb47-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5eb47-132">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5eb47-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5eb47-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5eb47-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5eb47-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5eb47-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5eb47-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
```
# <a name="c"></a>[<span data-ttu-id="5eb47-136">C#</span><span class="sxs-lookup"><span data-stu-id="5eb47-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5eb47-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5eb47-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5eb47-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5eb47-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5eb47-139">Java</span><span class="sxs-lookup"><span data-stu-id="5eb47-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5eb47-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5eb47-140">Response</span></span>
<span data-ttu-id="5eb47-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5eb47-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentDefaults"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "addedStudentAction": "none",
    "dueTime": "23:59:00",
    "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
  }
}
```

