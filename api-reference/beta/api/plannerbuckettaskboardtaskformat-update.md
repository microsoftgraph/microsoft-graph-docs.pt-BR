---
title: Atualizar plannerBucketTaskBoardTaskFormat
description: Atualize as propriedades do objeto **plannerBucketTaskBoardTaskFormat** .
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ff962e09e6bb603c20c25bc835c4ac980e237a08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538979"
---
# <a name="update-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="b403d-103">Atualizar plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="b403d-103">Update plannerBucketTaskBoardTaskFormat</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b403d-104">Atualize as propriedades do objeto **plannerBucketTaskBoardTaskFormat** .</span><span class="sxs-lookup"><span data-stu-id="b403d-104">Update the properties of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b403d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b403d-105">Permissions</span></span>
<span data-ttu-id="b403d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b403d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b403d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b403d-108">Permission type</span></span>      | <span data-ttu-id="b403d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b403d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b403d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b403d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b403d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b403d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b403d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b403d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b403d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b403d-113">Not supported.</span></span>    |
|<span data-ttu-id="b403d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b403d-114">Application</span></span> | <span data-ttu-id="b403d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b403d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b403d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b403d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /planner/tasks/<id>/bucketTaskBoardFormat
```
## <a name="optional-request-headers"></a><span data-ttu-id="b403d-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b403d-117">Optional request headers</span></span>
| <span data-ttu-id="b403d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="b403d-118">Name</span></span>       | <span data-ttu-id="b403d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="b403d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b403d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="b403d-120">Authorization</span></span>  | <span data-ttu-id="b403d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b403d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b403d-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="b403d-123">If-Match</span></span>  | <span data-ttu-id="b403d-124">Último valor de ETag conhecido para o **plannerBucketTaskBoardTaskFormat** a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b403d-124">Last known ETag value for the **plannerBucketTaskBoardTaskFormat** to be updated.</span></span> <span data-ttu-id="b403d-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b403d-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b403d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b403d-126">Request body</span></span>
<span data-ttu-id="b403d-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b403d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b403d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b403d-130">Property</span></span>     | <span data-ttu-id="b403d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b403d-131">Type</span></span>   |<span data-ttu-id="b403d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b403d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b403d-133">orderHint</span><span class="sxs-lookup"><span data-stu-id="b403d-133">orderHint</span></span>|<span data-ttu-id="b403d-134">String</span><span class="sxs-lookup"><span data-stu-id="b403d-134">String</span></span>|<span data-ttu-id="b403d-135">Dica usada para ordenar tarefas no modo de exibição de Bucket do quadro de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b403d-135">Hint used to order tasks in the Bucket view of the Task Board.</span></span> <span data-ttu-id="b403d-136">O formato é definido conforme descrito [aqui](../resources/planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="b403d-136">The format is defined as outlined [here](../resources/planner-order-hint-format.md).</span></span>|

## <a name="response"></a><span data-ttu-id="b403d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b403d-137">Response</span></span>

<span data-ttu-id="b403d-138">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b403d-138">If successful, this method returns a `200 OK` response code and updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="b403d-p106">Este método pode retornar qualquer um dos [códigos de status de HTTP](/graph/errors). Os erros mais comuns que os aplicativos devem tratar para esse método são as respostas 400, 403, 404, 409 e 412. Saiba mais sobre esses erros em [Condições de erro comuns do Planner](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="b403d-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b403d-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b403d-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b403d-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b403d-143">Request</span></span>
<span data-ttu-id="b403d-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b403d-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}-->
```http
PATCH https://graph.microsoft.com/beta/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat
Content-type: application/json
Content-length: 34
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="

{
  "orderHint": "A6673H Ejkl!"
}
```
##### <a name="response"></a><span data-ttu-id="b403d-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b403d-145">Response</span></span>
<span data-ttu-id="b403d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b403d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 68

{
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR",
  "orderHint": "C3665D"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update plannerbuckettaskboardtaskformat",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/plannerbuckettaskboardtaskformat-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
