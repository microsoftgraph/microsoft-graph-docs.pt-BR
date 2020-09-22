---
title: Atualizar educationAssignmentResource
description: 'Atualiza as propriedades do recurso associado a uma atribuição. Somente professores em uma classe podem alterar objetos de recurso de atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 17b1b6353c02633fbecdb8d480cb6f1411b31f40
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002475"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="21fce-104">Atualizar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="21fce-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="21fce-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21fce-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21fce-106">Atualiza as propriedades do recurso associado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="21fce-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="21fce-107">Somente professores em uma classe podem alterar objetos de recurso de atribuição.</span><span class="sxs-lookup"><span data-stu-id="21fce-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="21fce-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="21fce-108">Permissions</span></span>
<span data-ttu-id="21fce-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21fce-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21fce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21fce-111">Permission type</span></span>      | <span data-ttu-id="21fce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="21fce-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21fce-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21fce-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="21fce-114">EduAssignments. ReadWriteBasic, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21fce-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="21fce-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21fce-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="21fce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21fce-116">Not supported.</span></span>  |
|<span data-ttu-id="21fce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21fce-117">Application</span></span> | <span data-ttu-id="21fce-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21fce-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="21fce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21fce-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="21fce-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21fce-120">Request headers</span></span>
| <span data-ttu-id="21fce-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21fce-121">Header</span></span>       | <span data-ttu-id="21fce-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21fce-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21fce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21fce-123">Authorization</span></span>  | <span data-ttu-id="21fce-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21fce-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="21fce-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="21fce-126">Content-Type</span></span>  | <span data-ttu-id="21fce-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21fce-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21fce-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21fce-128">Request body</span></span>
<span data-ttu-id="21fce-129">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="21fce-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="21fce-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="21fce-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="21fce-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="21fce-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="21fce-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21fce-132">Property</span></span>     | <span data-ttu-id="21fce-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="21fce-133">Type</span></span>   |<span data-ttu-id="21fce-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="21fce-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21fce-135">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="21fce-135">distributeForStudentWork</span></span>|<span data-ttu-id="21fce-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="21fce-136">Boolean</span></span>| <span data-ttu-id="21fce-137">Indica se este recurso deve ser copiado para o objeto de recurso de cada aluno quando a atribuição é publicada.</span><span class="sxs-lookup"><span data-stu-id="21fce-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="21fce-138">recurso</span><span class="sxs-lookup"><span data-stu-id="21fce-138">resource</span></span>|<span data-ttu-id="21fce-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="21fce-139">educationResource</span></span>| <span data-ttu-id="21fce-140">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="21fce-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="21fce-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="21fce-141">Response</span></span>
<span data-ttu-id="21fce-142">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [educationAssignmentResource](../resources/educationassignmentresource.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21fce-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="21fce-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21fce-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21fce-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21fce-144">Request</span></span>
<span data-ttu-id="21fce-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="21fce-145">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="21fce-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="21fce-146">Response</span></span>
<span data-ttu-id="21fce-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="21fce-147">The following is an example of the response.</span></span> 

><span data-ttu-id="21fce-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21fce-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="21fce-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21fce-149">All of the properties will be returned from an actual call.</span></span>


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


