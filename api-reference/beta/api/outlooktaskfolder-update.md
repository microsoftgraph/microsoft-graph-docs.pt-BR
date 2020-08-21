---
title: Atualizar outlooktaskfolder
description: Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 948f633ae43d32a16322e60ad2cdf497642af828
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849734"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="80949-103">Atualizar outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="80949-103">Update outlooktaskfolder</span></span>

<span data-ttu-id="80949-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80949-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="80949-105">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="80949-105">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="80949-106">Você não pode alterar o valor da propriedade **Name** da pasta de tarefas padrão, "tarefas".</span><span class="sxs-lookup"><span data-stu-id="80949-106">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="80949-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="80949-107">Permissions</span></span>
<span data-ttu-id="80949-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80949-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80949-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80949-110">Permission type</span></span>      | <span data-ttu-id="80949-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80949-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80949-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80949-112">Delegated (work or school account)</span></span> | <span data-ttu-id="80949-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80949-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="80949-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80949-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80949-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80949-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="80949-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80949-116">Application</span></span> | <span data-ttu-id="80949-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80949-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="80949-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80949-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="80949-119">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="80949-119">Optional request headers</span></span>
| <span data-ttu-id="80949-120">Nome</span><span class="sxs-lookup"><span data-stu-id="80949-120">Name</span></span>       | <span data-ttu-id="80949-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="80949-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="80949-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80949-122">Authorization</span></span>  | <span data-ttu-id="80949-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80949-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80949-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80949-125">Request body</span></span>
<span data-ttu-id="80949-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="80949-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="80949-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80949-129">Property</span></span>     | <span data-ttu-id="80949-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80949-130">Type</span></span>   |<span data-ttu-id="80949-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80949-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80949-132">nome</span><span class="sxs-lookup"><span data-stu-id="80949-132">name</span></span>|<span data-ttu-id="80949-133">String</span><span class="sxs-lookup"><span data-stu-id="80949-133">String</span></span>|<span data-ttu-id="80949-134">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="80949-134">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="80949-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="80949-135">Response</span></span>

<span data-ttu-id="80949-136">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80949-136">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="80949-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80949-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="80949-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80949-138">Request</span></span>
<span data-ttu-id="80949-139">O exemplo a seguir altera o nome da pasta de tarefas especificada para `Charity work` .</span><span class="sxs-lookup"><span data-stu-id="80949-139">The following example changes the name of the specified task folder to `Charity work`.</span></span>

# <a name="http"></a>[<span data-ttu-id="80949-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="80949-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="80949-141">C#</span><span class="sxs-lookup"><span data-stu-id="80949-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80949-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80949-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80949-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80949-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="80949-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="80949-144">Response</span></span>
<span data-ttu-id="80949-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80949-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
