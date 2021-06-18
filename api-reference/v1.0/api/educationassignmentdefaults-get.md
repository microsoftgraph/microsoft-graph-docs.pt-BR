---
title: Obter educationAssignmentDefaults
description: Leia as propriedades e as relações de um objeto educationAssignmentDefaults.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c99f43ee19b40c0223d94ac4b9519b55bddcfcd3
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991224"
---
# <a name="get-educationassignmentdefaults"></a><span data-ttu-id="e35e6-103">Obter educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="e35e6-103">Get educationAssignmentDefaults</span></span>
<span data-ttu-id="e35e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e35e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e35e6-105">Leia as propriedades e as relações de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="e35e6-105">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> 

<span data-ttu-id="e35e6-106">Esses são os padrões de atribuição de nível de classe respeitados pelas novas atribuições criadas na classe.</span><span class="sxs-lookup"><span data-stu-id="e35e6-106">These are the class-level assignment defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="e35e6-107">Os chamadores podem continuar a especificar valores personalizados em cada criação de atribuição se não quiserem os comportamentos padrão.</span><span class="sxs-lookup"><span data-stu-id="e35e6-107">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="permissions"></a><span data-ttu-id="e35e6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e35e6-108">Permissions</span></span>
<span data-ttu-id="e35e6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e35e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e35e6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e35e6-111">Permission type</span></span>|<span data-ttu-id="e35e6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e35e6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e35e6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e35e6-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e35e6-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e35e6-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="e35e6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e35e6-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e35e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e35e6-116">Not supported.</span></span> |
|<span data-ttu-id="e35e6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e35e6-117">Application</span></span>| <span data-ttu-id="e35e6-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e35e6-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e35e6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e35e6-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e35e6-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e35e6-120">Optional query parameters</span></span>
<span data-ttu-id="e35e6-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e35e6-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e35e6-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e35e6-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e35e6-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e6-123">Request headers</span></span>
|<span data-ttu-id="e35e6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="e35e6-124">Name</span></span>|<span data-ttu-id="e35e6-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35e6-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e35e6-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e35e6-126">Authorization</span></span>|<span data-ttu-id="e35e6-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e35e6-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e35e6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e6-129">Request body</span></span>
<span data-ttu-id="e35e6-130">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="e35e6-130">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e35e6-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35e6-131">Response</span></span>

<span data-ttu-id="e35e6-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e35e6-132">If successful, this method returns a `200 OK` response code and an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e35e6-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e35e6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e35e6-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e35e6-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e35e6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="e35e6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentdefaults"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```
# <a name="c"></a>[<span data-ttu-id="e35e6-136">C#</span><span class="sxs-lookup"><span data-stu-id="e35e6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e35e6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e35e6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e35e6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e35e6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e35e6-139">Java</span><span class="sxs-lookup"><span data-stu-id="e35e6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e35e6-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e35e6-140">Response</span></span>
<span data-ttu-id="e35e6-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e35e6-141">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('c6f4e171-da1f-4598-a648-05fcec6cd9ba')"
  }
}
```

