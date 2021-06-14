---
title: Atualizar educationAssignmentSettings
description: Atualize as propriedades de um objeto educationAssignmentSettings.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11802b1b2fadfc717a123db31ad91436183442ed
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912229"
---
# <a name="update-educationassignmentsettings"></a><span data-ttu-id="eff0e-103">Atualizar educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="eff0e-103">Update educationAssignmentSettings</span></span>
<span data-ttu-id="eff0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="eff0e-105">Atualize as propriedades de [um objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="eff0e-105">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span> <span data-ttu-id="eff0e-106">Somente os professores podem atualizar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="eff0e-106">Only Teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="eff0e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="eff0e-107">Permissions</span></span>
<span data-ttu-id="eff0e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff0e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eff0e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eff0e-110">Permission type</span></span>|<span data-ttu-id="eff0e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eff0e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eff0e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eff0e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eff0e-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eff0e-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>|
|<span data-ttu-id="eff0e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eff0e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eff0e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff0e-115">Not supported.</span></span>|
|<span data-ttu-id="eff0e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eff0e-116">Application</span></span>|<span data-ttu-id="eff0e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eff0e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eff0e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eff0e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings
```

## <a name="request-headers"></a><span data-ttu-id="eff0e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eff0e-119">Request headers</span></span>
|<span data-ttu-id="eff0e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="eff0e-120">Name</span></span>|<span data-ttu-id="eff0e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eff0e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="eff0e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eff0e-122">Authorization</span></span>|<span data-ttu-id="eff0e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eff0e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="eff0e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eff0e-125">Content-Type</span></span>|<span data-ttu-id="eff0e-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eff0e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="eff0e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eff0e-128">Request body</span></span>
<span data-ttu-id="eff0e-129">No corpo da solicitação, fornece uma representação JSON do [objeto educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="eff0e-129">In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>

<span data-ttu-id="eff0e-130">A tabela a seguir mostra as propriedades que são necessárias ao atualizar [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span><span class="sxs-lookup"><span data-stu-id="eff0e-130">The following table shows the properties that are required when you update the [educationAssignmentSettings](../resources/educationassignmentsettings.md).</span></span>

|<span data-ttu-id="eff0e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eff0e-131">Property</span></span>|<span data-ttu-id="eff0e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="eff0e-132">Type</span></span>|<span data-ttu-id="eff0e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="eff0e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eff0e-134">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="eff0e-134">submissionAnimationDisabled</span></span>|<span data-ttu-id="eff0e-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="eff0e-135">Boolean</span></span>|<span data-ttu-id="eff0e-136">Indica se a animação de celebração de turn-in será mostrada.</span><span class="sxs-lookup"><span data-stu-id="eff0e-136">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="eff0e-137">Um valor `true` indica que a animação não será mostrada.</span><span class="sxs-lookup"><span data-stu-id="eff0e-137">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="eff0e-138">O valor padrão é `false`.</span><span class="sxs-lookup"><span data-stu-id="eff0e-138">Default value is `false`.</span></span>|



## <a name="response"></a><span data-ttu-id="eff0e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff0e-139">Response</span></span>

<span data-ttu-id="eff0e-140">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentSettings](../resources/educationassignmentsettings.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eff0e-140">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eff0e-141">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eff0e-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eff0e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eff0e-142">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="eff0e-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="eff0e-143">Response</span></span>
<span data-ttu-id="eff0e-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="eff0e-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

