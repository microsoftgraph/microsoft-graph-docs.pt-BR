---
title: Obter educationAssignmentSettings
description: Leia as propriedades e as relações de um objeto educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fbc7a5c17c0d980de9baa95d625d7bb058b167e9
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912141"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="ed7a3-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ed7a3-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="ed7a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed7a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed7a3-105">Leia as propriedades e as relações de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ed7a3-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed7a3-106">Permissions</span></span>
<span data-ttu-id="ed7a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed7a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed7a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed7a3-109">Permission type</span></span>|<span data-ttu-id="ed7a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed7a3-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed7a3-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed7a3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed7a3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed7a3-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="ed7a3-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed7a3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed7a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-114">Not supported.</span></span>|
|<span data-ttu-id="ed7a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed7a3-115">Application</span></span>| <span data-ttu-id="ed7a3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ed7a3-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed7a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed7a3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed7a3-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ed7a3-118">Optional query parameters</span></span>
<span data-ttu-id="ed7a3-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ed7a3-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ed7a3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed7a3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7a3-121">Request headers</span></span>
|<span data-ttu-id="ed7a3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ed7a3-122">Name</span></span>|<span data-ttu-id="ed7a3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed7a3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed7a3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed7a3-124">Authorization</span></span>|<span data-ttu-id="ed7a3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed7a3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7a3-127">Request body</span></span>
<span data-ttu-id="ed7a3-128">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed7a3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed7a3-129">Response</span></span>

<span data-ttu-id="ed7a3-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed7a3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed7a3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed7a3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed7a3-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

### <a name="response"></a><span data-ttu-id="ed7a3-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed7a3-133">Response</span></span>
<span data-ttu-id="ed7a3-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ed7a3-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

