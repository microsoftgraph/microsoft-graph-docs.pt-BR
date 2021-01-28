---
title: Obter educationAssignmentSettings
description: Leia as propriedades e os relacionamentos de um objeto educationAssignmentSettings.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 896e47bded7ee5d34a2b923107737feafbf37144
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034322"
---
# <a name="get-educationassignmentsettings"></a><span data-ttu-id="2c6a2-103">Obter educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2c6a2-103">Get educationAssignmentSettings</span></span>
<span data-ttu-id="2c6a2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c6a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c6a2-105">Leia as propriedades e os relacionamentos de um [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2c6a2-105">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c6a2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c6a2-106">Permissions</span></span>
<span data-ttu-id="2c6a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c6a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c6a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c6a2-109">Permission type</span></span>|<span data-ttu-id="2c6a2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c6a2-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2c6a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c6a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2c6a2-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c6a2-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="2c6a2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c6a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c6a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-114">Not supported.</span></span>|
|<span data-ttu-id="2c6a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c6a2-115">Application</span></span>|<span data-ttu-id="2c6a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c6a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c6a2-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{id}/assignmentSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c6a2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2c6a2-118">Optional query parameters</span></span>
<span data-ttu-id="2c6a2-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2c6a2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2c6a2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2c6a2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6a2-121">Request headers</span></span>
|<span data-ttu-id="2c6a2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2c6a2-122">Name</span></span>|<span data-ttu-id="2c6a2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6a2-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2c6a2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c6a2-124">Authorization</span></span>|<span data-ttu-id="2c6a2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c6a2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6a2-127">Request body</span></span>
<span data-ttu-id="2c6a2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c6a2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6a2-129">Response</span></span>

<span data-ttu-id="2c6a2-130">Se bem-sucedido, este método retorna um código de resposta e um objeto `200 OK` [educationAssignmentSettings](../resources/educationassignmentsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-130">If successful, this method returns a `200 OK` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c6a2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c6a2-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c6a2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c6a2-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentSettings
```

### <a name="response"></a><span data-ttu-id="2c6a2-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c6a2-133">Response</span></span>
<span data-ttu-id="2c6a2-134">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2c6a2-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

