---
title: Atualizar educationAssignmentDefaults
description: Atualize as propriedades de um objeto educationAssignmentDefaults.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4dd6d6d8d2c5433ca2ad133c57cae8b17af79ad5
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780817"
---
# <a name="update-educationassignmentdefaults"></a><span data-ttu-id="73e96-103">Atualizar educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="73e96-103">Update educationAssignmentDefaults</span></span>
<span data-ttu-id="73e96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73e96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73e96-105">Atualize as propriedades de um [objeto educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="73e96-105">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span> <span data-ttu-id="73e96-106">Somente os professores podem atualizar essas configurações.</span><span class="sxs-lookup"><span data-stu-id="73e96-106">Only teachers can update these settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="73e96-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="73e96-107">Permissions</span></span>
<span data-ttu-id="73e96-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73e96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73e96-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73e96-110">Permission type</span></span>|<span data-ttu-id="73e96-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73e96-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73e96-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73e96-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="73e96-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73e96-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="73e96-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73e96-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="73e96-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73e96-115">Not supported.</span></span>  |
|<span data-ttu-id="73e96-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73e96-116">Application</span></span> | <span data-ttu-id="73e96-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73e96-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73e96-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73e96-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /education/classes/{id}/assignmentDefaults
```

## <a name="request-headers"></a><span data-ttu-id="73e96-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73e96-119">Request headers</span></span>
|<span data-ttu-id="73e96-120">Nome</span><span class="sxs-lookup"><span data-stu-id="73e96-120">Name</span></span>|<span data-ttu-id="73e96-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e96-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="73e96-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73e96-122">Authorization</span></span>|<span data-ttu-id="73e96-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73e96-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="73e96-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73e96-125">Content-Type</span></span>|<span data-ttu-id="73e96-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73e96-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73e96-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73e96-128">Request body</span></span>
<span data-ttu-id="73e96-129">No corpo da solicitação, fornece os valores para campos relevantes do [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="73e96-129">In the request body, supply the values for relevant fields of the [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object that should be updated.</span></span> <span data-ttu-id="73e96-130">As propriedades existentes que não estão incluídas no corpo da solicitação manterão seus valores anteriores.</span><span class="sxs-lookup"><span data-stu-id="73e96-130">Existing properties that are not included in the request body will maintain their previous values.</span></span> <span data-ttu-id="73e96-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="73e96-131">For best performance, don't include existing values that haven't changed.</span></span>

|<span data-ttu-id="73e96-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73e96-132">Property</span></span>|<span data-ttu-id="73e96-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="73e96-133">Type</span></span>|<span data-ttu-id="73e96-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="73e96-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73e96-135">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="73e96-135">addedStudentAction</span></span>|<span data-ttu-id="73e96-136">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="73e96-136">educationAddedStudentAction</span></span>|<span data-ttu-id="73e96-137">Comportamento padrão no nível de classe para lidar com alunos que são adicionados após a publicação da atribuição.</span><span class="sxs-lookup"><span data-stu-id="73e96-137">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="73e96-138">Os valores possíveis são: `none` e `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="73e96-138">Possible values are: `none`, `assignIfOpen`.</span></span> <span data-ttu-id="73e96-139">O valor padrão é `none`.</span><span class="sxs-lookup"><span data-stu-id="73e96-139">The default value is `none`.</span></span>|
|<span data-ttu-id="73e96-140">dueTime</span><span class="sxs-lookup"><span data-stu-id="73e96-140">dueTime</span></span>|<span data-ttu-id="73e96-141">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="73e96-141">TimeOfDay</span></span>|<span data-ttu-id="73e96-142">Valor padrão de nível de classe para o campo de tempo de vencimento.</span><span class="sxs-lookup"><span data-stu-id="73e96-142">Class-level default value for due time field.</span></span> <span data-ttu-id="73e96-143">O valor padrão é `23:59:00`</span><span class="sxs-lookup"><span data-stu-id="73e96-143">Default value is `23:59:00`</span></span>|
|<span data-ttu-id="73e96-144">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="73e96-144">notificationChannelUrl</span></span>|<span data-ttu-id="73e96-145">String</span><span class="sxs-lookup"><span data-stu-id="73e96-145">String</span></span>|<span data-ttu-id="73e96-146">Canal Teams padrão para o qual as notificações serão enviadas.</span><span class="sxs-lookup"><span data-stu-id="73e96-146">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="73e96-147">O valor padrão é `null`.</span><span class="sxs-lookup"><span data-stu-id="73e96-147">Default value is `null`.</span></span>|



## <a name="response"></a><span data-ttu-id="73e96-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e96-148">Response</span></span>

<span data-ttu-id="73e96-149">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto educationAssignmentDefaults](../resources/educationassignmentdefaults.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73e96-149">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73e96-150">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73e96-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="73e96-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73e96-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="73e96-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="73e96-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentdefaults"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{id}/assignmentDefaults
Content-Type: application/json
Content-length: 181

{
  "addedStudentAction": "assignIfOpen",
  "addToCalendarAction": "studentsAndTeamOwners",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```
# <a name="c"></a>[<span data-ttu-id="73e96-153">C#</span><span class="sxs-lookup"><span data-stu-id="73e96-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignmentdefaults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73e96-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73e96-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignmentdefaults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73e96-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73e96-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignmentdefaults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73e96-156">Java</span><span class="sxs-lookup"><span data-stu-id="73e96-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignmentdefaults-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="73e96-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="73e96-157">Response</span></span>
<span data-ttu-id="73e96-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="73e96-158">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "addToCalendarAction": "studentsAndTeamOwners",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

