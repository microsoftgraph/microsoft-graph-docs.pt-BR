---
title: Atualizar outlooktaskfolder
description: Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9b7727ce554e5dccb24dae78e73d4692330691dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337897"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="36cd5-103">Atualizar outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="36cd5-103">Update outlooktaskfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36cd5-104">Atualizar as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="36cd5-104">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="36cd5-105">Você não pode alterar o valor da propriedade **Name** da pasta de tarefas padrão, "tarefas".</span><span class="sxs-lookup"><span data-stu-id="36cd5-105">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="36cd5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="36cd5-106">Permissions</span></span>
<span data-ttu-id="36cd5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36cd5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36cd5-109">Permission type</span></span>      | <span data-ttu-id="36cd5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36cd5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36cd5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36cd5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="36cd5-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36cd5-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="36cd5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36cd5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36cd5-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="36cd5-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="36cd5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36cd5-115">Application</span></span> | <span data-ttu-id="36cd5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36cd5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36cd5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36cd5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="36cd5-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="36cd5-118">Optional request headers</span></span>
| <span data-ttu-id="36cd5-119">Name</span><span class="sxs-lookup"><span data-stu-id="36cd5-119">Name</span></span>       | <span data-ttu-id="36cd5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="36cd5-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="36cd5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="36cd5-121">Authorization</span></span>  | <span data-ttu-id="36cd5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36cd5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36cd5-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36cd5-124">Request body</span></span>
<span data-ttu-id="36cd5-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="36cd5-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="36cd5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36cd5-128">Property</span></span>     | <span data-ttu-id="36cd5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="36cd5-129">Type</span></span>   |<span data-ttu-id="36cd5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="36cd5-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36cd5-131">name</span><span class="sxs-lookup"><span data-stu-id="36cd5-131">name</span></span>|<span data-ttu-id="36cd5-132">String</span><span class="sxs-lookup"><span data-stu-id="36cd5-132">String</span></span>|<span data-ttu-id="36cd5-133">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="36cd5-133">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="36cd5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cd5-134">Response</span></span>

<span data-ttu-id="36cd5-135">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [outlookTaskFolder](../resources/outlooktaskfolder.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36cd5-135">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36cd5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36cd5-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36cd5-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36cd5-137">Request</span></span>
<span data-ttu-id="36cd5-138">O exemplo a seguir altera o nome da pasta de tarefas especificada `Charity work`para.</span><span class="sxs-lookup"><span data-stu-id="36cd5-138">The following example changes the name of the specified task folder to `Charity work`.</span></span>
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
##### <a name="response"></a><span data-ttu-id="36cd5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="36cd5-139">Response</span></span>
<span data-ttu-id="36cd5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36cd5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
