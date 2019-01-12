---
title: Atualizar outlooktaskfolder
description: Atualize as propriedades graváveis de uma pasta de tarefas do Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: af86b85df5529f7f8c15ce2e4977d4b0fe2f00ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925676"
---
# <a name="update-outlooktaskfolder"></a><span data-ttu-id="de760-103">Atualizar outlooktaskfolder</span><span class="sxs-lookup"><span data-stu-id="de760-103">Update outlooktaskfolder</span></span>

> <span data-ttu-id="de760-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="de760-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de760-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="de760-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de760-106">Atualize as propriedades graváveis de uma pasta de tarefas do Outlook.</span><span class="sxs-lookup"><span data-stu-id="de760-106">Update the writable properties of an Outlook task folder.</span></span>

<span data-ttu-id="de760-107">Você não pode alterar o valor da propriedade de **nome** da pasta de tarefas padrão, "Tarefas".</span><span class="sxs-lookup"><span data-stu-id="de760-107">You cannot change the **name** property value of the default task folder, "Tasks".</span></span>
## <a name="permissions"></a><span data-ttu-id="de760-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="de760-108">Permissions</span></span>
<span data-ttu-id="de760-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de760-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de760-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de760-111">Permission type</span></span>      | <span data-ttu-id="de760-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de760-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de760-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de760-113">Delegated (work or school account)</span></span> | <span data-ttu-id="de760-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de760-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="de760-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de760-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de760-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de760-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="de760-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de760-117">Application</span></span> | <span data-ttu-id="de760-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de760-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de760-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de760-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="de760-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="de760-120">Optional request headers</span></span>
| <span data-ttu-id="de760-121">Nome</span><span class="sxs-lookup"><span data-stu-id="de760-121">Name</span></span>       | <span data-ttu-id="de760-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de760-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="de760-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="de760-123">Authorization</span></span>  | <span data-ttu-id="de760-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de760-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de760-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de760-126">Request body</span></span>
<span data-ttu-id="de760-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="de760-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="de760-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de760-130">Property</span></span>     | <span data-ttu-id="de760-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="de760-131">Type</span></span>   |<span data-ttu-id="de760-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="de760-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de760-133">name</span><span class="sxs-lookup"><span data-stu-id="de760-133">name</span></span>|<span data-ttu-id="de760-134">String</span><span class="sxs-lookup"><span data-stu-id="de760-134">String</span></span>|<span data-ttu-id="de760-135">O nome da pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="de760-135">The name of the task folder.</span></span>|

## <a name="response"></a><span data-ttu-id="de760-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="de760-136">Response</span></span>

<span data-ttu-id="de760-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [outlookTaskFolder](../resources/outlooktaskfolder.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de760-137">If successful, this method returns a `200 OK` response code and updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de760-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de760-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de760-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de760-139">Request</span></span>
<span data-ttu-id="de760-140">O exemplo a seguir altera o nome da pasta tarefa especificada a `Charity work`.</span><span class="sxs-lookup"><span data-stu-id="de760-140">The following example changes the name of the specified task folder to `Charity work`.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPWAAA=')
Content-type: application/json
Content-length: 31

{
  "name": "Charity work"
}
```
##### <a name="response"></a><span data-ttu-id="de760-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="de760-141">Response</span></span>
<span data-ttu-id="de760-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de760-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update outlooktaskfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
