---
title: Obter onenoteOperation
description: 'Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: c869702b856f03bccbbc5101e8e72facd3287738
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932382"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="6554f-104">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="6554f-104">Get onenoteOperation</span></span>

<span data-ttu-id="6554f-p102">Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="6554f-p102">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="6554f-107">Você pode sondar o ponto de extremidade de Operation-Location até a propriedade `status` retornar `completed` ou `failed`.</span><span class="sxs-lookup"><span data-stu-id="6554f-107">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="6554f-108">Se o status for `completed`, a propriedade `resourceLocation` conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="6554f-108">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="6554f-109">Se o status for `failed`, o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="6554f-109">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="6554f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="6554f-110">Permissions</span></span>
<span data-ttu-id="6554f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6554f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6554f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6554f-113">Permission type</span></span>      | <span data-ttu-id="6554f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6554f-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6554f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6554f-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6554f-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6554f-116">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="6554f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6554f-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6554f-118">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6554f-118">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="6554f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6554f-119">Application</span></span> | <span data-ttu-id="6554f-120">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6554f-120">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6554f-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6554f-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6554f-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6554f-122">Optional query parameters</span></span>
<span data-ttu-id="6554f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6554f-123">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6554f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6554f-124">Request headers</span></span>
| <span data-ttu-id="6554f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="6554f-125">Name</span></span>       | <span data-ttu-id="6554f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6554f-126">Type</span></span> | <span data-ttu-id="6554f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6554f-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6554f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="6554f-128">Authorization</span></span>  | <span data-ttu-id="6554f-129">string</span><span class="sxs-lookup"><span data-stu-id="6554f-129">string</span></span>  | <span data-ttu-id="6554f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6554f-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6554f-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6554f-132">Accept</span></span> | <span data-ttu-id="6554f-133">string</span><span class="sxs-lookup"><span data-stu-id="6554f-133">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="6554f-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6554f-134">Request body</span></span>
<span data-ttu-id="6554f-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6554f-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6554f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="6554f-136">Response</span></span>

<span data-ttu-id="6554f-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6554f-137">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6554f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6554f-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6554f-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6554f-139">Request</span></span>
<span data-ttu-id="6554f-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6554f-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="6554f-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6554f-141">Response</span></span>
<span data-ttu-id="6554f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6554f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "id": "id-value",
  "status": "status-value",
  "createdDateTime": "2016-10-19T10:37:00Z",
  "lastActionDateTime": "2016-10-19T10:37:00Z",
  "resourceLocation": "resourceLocation-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get onenoteOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
