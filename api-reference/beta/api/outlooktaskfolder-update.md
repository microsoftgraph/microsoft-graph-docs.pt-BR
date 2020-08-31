---
title: Atualizar outlooktaskfolder
description: Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 99c3ca379760812ad3312395b3f03d2bdaf3d2a8
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311950"
---
# <a name="update-outlooktaskfolder-deprecated"></a><span data-ttu-id="b617b-103">Atualizar outlooktaskfolder (preterido)</span><span class="sxs-lookup"><span data-stu-id="b617b-103">Update outlooktaskfolder (deprecated)</span></span>

<span data-ttu-id="b617b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b617b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="b617b-105">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="b617b-105">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="b617b-106">Você não pode alterar o valor da propriedade **Name** da pasta de tarefas padrão, "tarefas".</span><span class="sxs-lookup"><span data-stu-id="b617b-106">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="b617b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b617b-107">Permissions</span></span>
<span data-ttu-id="b617b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b617b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b617b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b617b-110">Permission type</span></span>      | <span data-ttu-id="b617b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b617b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b617b-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b617b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b617b-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b617b-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b617b-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b617b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b617b-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b617b-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="b617b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b617b-116">Application</span></span> | <span data-ttu-id="b617b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b617b-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b617b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b617b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b617b-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="b617b-119">Optional request headers</span></span>
| <span data-ttu-id="b617b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="b617b-120">Name</span></span>       | <span data-ttu-id="b617b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="b617b-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b617b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b617b-122">Authorization</span></span>  | <span data-ttu-id="b617b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b617b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b617b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b617b-125">Request body</span></span>
<span data-ttu-id="b617b-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b617b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b617b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b617b-129">Property</span></span>     | <span data-ttu-id="b617b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b617b-130">Type</span></span>   |<span data-ttu-id="b617b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b617b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b617b-132">nome</span><span class="sxs-lookup"><span data-stu-id="b617b-132">name</span></span>|<span data-ttu-id="b617b-133">String</span><span class="sxs-lookup"><span data-stu-id="b617b-133">String</span></span>|<span data-ttu-id="b617b-134">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="b617b-134">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="b617b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="b617b-135">Response</span></span>

<span data-ttu-id="b617b-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b617b-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b617b-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b617b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b617b-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b617b-138">Request</span></span>
<span data-ttu-id="b617b-139">O exemplo a seguir altera o nome da pasta de tarefas especificada para `Charity work` .</span><span class="sxs-lookup"><span data-stu-id="b617b-139">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="http"></a>[<span data-ttu-id="b617b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b617b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
# <a name="c"></a>[<span data-ttu-id="b617b-141">C#</span><span class="sxs-lookup"><span data-stu-id="b617b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b617b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b617b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b617b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b617b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b617b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="b617b-144">Response</span></span>
<span data-ttu-id="b617b-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b617b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAhrbPWAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAKfQ==",
  "isDefaultFolder": false,
  "name": "Charity work",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
