---
title: Atualizar educationAssignmentSettings
description: Atualize as propriedades de um objeto educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7c251885de43022f8e3065c7004dab33d4fa78a8
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992965"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="8b1f0-103">Atualizar educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="8b1f0-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="8b1f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b1f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8b1f0-105">Atualize as propriedades de [um objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8b1f0-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="8b1f0-106">Somente os professores podem atualizar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b1f0-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="8b1f0-107">Permissions</span></span>
<span data-ttu-id="8b1f0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b1f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b1f0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b1f0-110">Permission type</span></span>|<span data-ttu-id="8b1f0-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b1f0-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b1f0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b1f0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b1f0-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b1f0-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="8b1f0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b1f0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b1f0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-115">Not supported.</span></span>|
|<span data-ttu-id="8b1f0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b1f0-116">Application</span></span>|<span data-ttu-id="8b1f0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b1f0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1f0-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="8b1f0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1f0-119">Request headers</span></span>
|<span data-ttu-id="8b1f0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="8b1f0-120">Name</span></span>|<span data-ttu-id="8b1f0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b1f0-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8b1f0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b1f0-122">Authorization</span></span>|<span data-ttu-id="8b1f0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8b1f0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8b1f0-125">Content-Type</span></span>|<span data-ttu-id="8b1f0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b1f0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1f0-128">Request body</span></span>
<span data-ttu-id="8b1f0-129">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8b1f0-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="8b1f0-130">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="8b1f0-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="8b1f0-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b1f0-131">Property</span></span>|<span data-ttu-id="8b1f0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b1f0-132">Type</span></span>|<span data-ttu-id="8b1f0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b1f0-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b1f0-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="8b1f0-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="8b1f0-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b1f0-135">Boolean</span></span>|<span data-ttu-id="8b1f0-136">Indica se a animação de celebração de turn-in será mostrada.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="8b1f0-137">Um valor `true` indica que a animação não será mostrada.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="8b1f0-138">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="8b1f0-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1f0-139">Response</span></span>

<span data-ttu-id="8b1f0-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b1f0-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b1f0-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8b1f0-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b1f0-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="8b1f0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="8b1f0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "submissionAnimationDisabled": true
}
```
# <a name="c"></a>[<span data-ttu-id="8b1f0-144">C#</span><span class="sxs-lookup"><span data-stu-id="8b1f0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8b1f0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8b1f0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8b1f0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8b1f0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8b1f0-147">Java</span><span class="sxs-lookup"><span data-stu-id="8b1f0-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8b1f0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b1f0-148">Response</span></span>
<span data-ttu-id="8b1f0-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b1f0-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "submissionAnimationDisabled": true
}
```

