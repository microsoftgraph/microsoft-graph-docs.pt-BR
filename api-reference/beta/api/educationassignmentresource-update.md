---
title: Atualizar educationAssignmentResource
description: 'Atualiza as propriedades do recurso associado a uma atribuição. Somente professores em uma classe podem alterar objetos de recurso de atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d3ce0db2353d91f17f059fe8a2dfd9d6c775e1e2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324643"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="4c26b-104">Atualizar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="4c26b-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c26b-105">Atualiza as propriedades do recurso associado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="4c26b-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="4c26b-106">Somente professores em uma classe podem alterar objetos de recurso de atribuição.</span><span class="sxs-lookup"><span data-stu-id="4c26b-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="4c26b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="4c26b-107">Permissions</span></span>
<span data-ttu-id="4c26b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c26b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c26b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c26b-110">Permission type</span></span>      | <span data-ttu-id="4c26b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4c26b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c26b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c26b-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c26b-113">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c26b-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="4c26b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c26b-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c26b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c26b-115">Not supported.</span></span>  |
|<span data-ttu-id="4c26b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c26b-116">Application</span></span> | <span data-ttu-id="4c26b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c26b-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4c26b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c26b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4c26b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c26b-119">Request headers</span></span>
| <span data-ttu-id="4c26b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c26b-120">Header</span></span>       | <span data-ttu-id="4c26b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4c26b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c26b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c26b-122">Authorization</span></span>  | <span data-ttu-id="4c26b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c26b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4c26b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c26b-125">Content-Type</span></span>  | <span data-ttu-id="4c26b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c26b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c26b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c26b-127">Request body</span></span>
<span data-ttu-id="4c26b-128">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="4c26b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c26b-129">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="4c26b-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c26b-130">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="4c26b-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c26b-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c26b-131">Property</span></span>     | <span data-ttu-id="4c26b-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c26b-132">Type</span></span>   |<span data-ttu-id="4c26b-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c26b-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c26b-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="4c26b-134">distributeForStudentWork</span></span>|<span data-ttu-id="4c26b-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c26b-135">Boolean</span></span>| <span data-ttu-id="4c26b-136">Indica se este recurso deve ser copiado para o objeto de recurso de cada aluno quando a atribuição é publicada.</span><span class="sxs-lookup"><span data-stu-id="4c26b-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="4c26b-137">recurso</span><span class="sxs-lookup"><span data-stu-id="4c26b-137">resource</span></span>|<span data-ttu-id="4c26b-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="4c26b-138">educationResource</span></span>| <span data-ttu-id="4c26b-139">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="4c26b-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="4c26b-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c26b-140">Response</span></span>
<span data-ttu-id="4c26b-141">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c26b-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c26b-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c26b-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c26b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c26b-143">Request</span></span>
<span data-ttu-id="4c26b-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c26b-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
##### <a name="response"></a><span data-ttu-id="4c26b-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c26b-145">Response</span></span>
<span data-ttu-id="4c26b-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4c26b-146">The following is an example of the response.</span></span> 

><span data-ttu-id="4c26b-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4c26b-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4c26b-148">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c26b-148">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

{
  "distributeForStudentWork": false,
  "resource": {
      "@odata.type": "#microsoft.graph.educationLinkResource",
      "displayName": "Microsoft Homepage",
      "createdDateTime": "2017-10-21T07:52:45.5675913Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "link": "https://www.microsoft.com"
  },
  "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
