---
title: Atualizar educationAssignmentResource
description: 'Atualize as propriedades de recurso associado a uma atribuição. Somente professores em uma classe podem alterar os objetos de recurso de atribuição.  '
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 91321cc124baa87a82f2f1f5fecc65365cafc18d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879307"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="8818f-104">Atualizar educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="8818f-104">Update educationAssignmentResource</span></span>

> <span data-ttu-id="8818f-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8818f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8818f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8818f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8818f-107">Atualize as propriedades de recurso associado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="8818f-107">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="8818f-108">Somente professores em uma classe podem alterar os objetos de recurso de atribuição.</span><span class="sxs-lookup"><span data-stu-id="8818f-108">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="8818f-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8818f-109">Permissions</span></span>
<span data-ttu-id="8818f-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8818f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8818f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8818f-112">Permission type</span></span>      | <span data-ttu-id="8818f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8818f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8818f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8818f-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="8818f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8818f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8818f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8818f-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8818f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8818f-117">Not supported.</span></span>  |
|<span data-ttu-id="8818f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8818f-118">Application</span></span> | <span data-ttu-id="8818f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8818f-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8818f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8818f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8818f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8818f-121">Request headers</span></span>
| <span data-ttu-id="8818f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8818f-122">Header</span></span>       | <span data-ttu-id="8818f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8818f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8818f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8818f-124">Authorization</span></span>  | <span data-ttu-id="8818f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8818f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8818f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8818f-127">Content-Type</span></span>  | <span data-ttu-id="8818f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="8818f-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8818f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8818f-129">Request body</span></span>
<span data-ttu-id="8818f-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="8818f-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8818f-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="8818f-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="8818f-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="8818f-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8818f-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8818f-133">Property</span></span>     | <span data-ttu-id="8818f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="8818f-134">Type</span></span>   |<span data-ttu-id="8818f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8818f-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8818f-136">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="8818f-136">distributeForStudentWork</span></span>|<span data-ttu-id="8818f-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="8818f-137">Boolean</span></span>| <span data-ttu-id="8818f-138">Indica se este recurso deve ser copiado para o objeto de recurso de cada student quando a atribuição é publicada.</span><span class="sxs-lookup"><span data-stu-id="8818f-138">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="8818f-139">recurso</span><span class="sxs-lookup"><span data-stu-id="8818f-139">resource</span></span>|<span data-ttu-id="8818f-140">educationResource</span><span class="sxs-lookup"><span data-stu-id="8818f-140">educationResource</span></span>| <span data-ttu-id="8818f-141">Objeto Resource.</span><span class="sxs-lookup"><span data-stu-id="8818f-141">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="8818f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="8818f-142">Response</span></span>
<span data-ttu-id="8818f-143">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [educationAssignmentResource](../resources/educationassignmentresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8818f-143">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8818f-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8818f-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8818f-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8818f-145">Request</span></span>
<span data-ttu-id="8818f-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8818f-146">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="8818f-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="8818f-147">Response</span></span>
<span data-ttu-id="8818f-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8818f-148">The following is an example of the response.</span></span> 

><span data-ttu-id="8818f-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8818f-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8818f-150">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8818f-150">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
