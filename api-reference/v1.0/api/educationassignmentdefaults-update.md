---
title: Atualizar educationAssignmentDefaults
description: Atualize as propriedades de um objeto educationAssignmentDefaults.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7f73af01d485bfade10dfae769290eb40a36c656
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911367"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="a96c1-103">Atualizar educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="a96c1-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="a96c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a96c1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a96c1-105">Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="a96c1-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>

<span data-ttu-id="a96c1-106">Somente os professores podem atualizar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="a96c1-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="a96c1-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a96c1-107">Permissions</span></span>
<span data-ttu-id="a96c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a96c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a96c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a96c1-110">Permission type</span></span>|<span data-ttu-id="a96c1-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a96c1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a96c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a96c1-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="a96c1-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a96c1-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a96c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a96c1-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a96c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a96c1-115">Not supported.</span></span>  |
|<span data-ttu-id="a96c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a96c1-116">Application</span></span> | <span data-ttu-id="a96c1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a96c1-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a96c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a96c1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="a96c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a96c1-119">Request headers</span></span>
|<span data-ttu-id="a96c1-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a96c1-120">Name</span></span>|<span data-ttu-id="a96c1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a96c1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a96c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a96c1-122">Authorization</span></span>|<span data-ttu-id="a96c1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a96c1-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a96c1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a96c1-125">Content-Type</span></span>|<span data-ttu-id="a96c1-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a96c1-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a96c1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a96c1-128">Request body</span></span>
<span data-ttu-id="a96c1-129">No corpo da solicitação, fornece apenas os valores dos campos que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="a96c1-129">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="a96c1-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a96c1-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a96c1-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a96c1-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="a96c1-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a96c1-132">Property</span></span>|<span data-ttu-id="a96c1-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a96c1-133">Type</span></span>|<span data-ttu-id="a96c1-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a96c1-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a96c1-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="a96c1-135">addedStudentAction</span></span>|<span data-ttu-id="a96c1-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="a96c1-136">educationAddedStudentAction</span></span>| <span data-ttu-id="a96c1-137">Ações padrão de nível de classe para alunos adicionados após a data de publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="a96c1-137">Class-level default actions for students added after the assignment publication date.</span></span> <span data-ttu-id="a96c1-138">Os valores possíveis são: `none` e `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="a96c1-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="a96c1-139">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="a96c1-139">The default value is `none`.</span></span>|
|<span data-ttu-id="a96c1-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="a96c1-140">dueTime</span></span>|<span data-ttu-id="a96c1-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a96c1-141">TimeOfDay</span></span>| <span data-ttu-id="a96c1-142">Valor padrão de nível de classe para o campo de tempo de vencimento.</span><span class="sxs-lookup"><span data-stu-id="a96c1-142">Class-level default value for due time field.</span></span> <span data-ttu-id="a96c1-143">O valor padrão é `23:59:00`</span><span class="sxs-lookup"><span data-stu-id="a96c1-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="a96c1-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="a96c1-144">notificationChannelUrl</span></span>|<span data-ttu-id="a96c1-145">String</span><span class="sxs-lookup"><span data-stu-id="a96c1-145">String</span></span>| <span data-ttu-id="a96c1-146">Canal Teams padrão para enviar notificações relacionadas à atribuição.</span><span class="sxs-lookup"><span data-stu-id="a96c1-146">Default Teams channel to send notifications related to the assignment.</span></span> <span data-ttu-id="a96c1-147">O valor padrão é `null`.</span><span class="sxs-lookup"><span data-stu-id="a96c1-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="a96c1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96c1-148">Response</span></span>

<span data-ttu-id="a96c1-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a96c1-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a96c1-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a96c1-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a96c1-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a96c1-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```

### <a name="response"></a><span data-ttu-id="a96c1-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="a96c1-152">Response</span></span>
<span data-ttu-id="a96c1-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a96c1-153">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "addedStudentAction": "assignIfOpen",
  "dueTime": "String",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}
```

