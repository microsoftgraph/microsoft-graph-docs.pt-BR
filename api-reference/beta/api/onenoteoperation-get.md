---
title: Obter onenoteOperation
description: 'Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
ms.openlocfilehash: abd11846cce1eab5e51ffc966d754a8a47f005bb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039147"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="e1fe5-104">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="e1fe5-104">Get onenoteOperation</span></span>

> <span data-ttu-id="e1fe5-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1fe5-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1fe5-p103">Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="e1fe5-109">Você pode sondar o ponto de extremidade de Operation-Location até a propriedade `status` retornar `completed` ou `failed`.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="e1fe5-110">Se o status for `completed`, a propriedade `resourceLocation` conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="e1fe5-111">Se o status for `failed`, o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1fe5-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1fe5-112">Permissions</span></span>
<span data-ttu-id="e1fe5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1fe5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1fe5-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1fe5-115">Permission type</span></span>      | <span data-ttu-id="e1fe5-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1fe5-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1fe5-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1fe5-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e1fe5-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fe5-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1fe5-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1fe5-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1fe5-120">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1fe5-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="e1fe5-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1fe5-121">Application</span></span> | <span data-ttu-id="e1fe5-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1fe5-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1fe5-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1fe5-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e1fe5-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1fe5-124">Optional query parameters</span></span>
<span data-ttu-id="e1fe5-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1fe5-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1fe5-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fe5-126">Request headers</span></span>
| <span data-ttu-id="e1fe5-127">Nome</span><span class="sxs-lookup"><span data-stu-id="e1fe5-127">Name</span></span>       | <span data-ttu-id="e1fe5-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1fe5-128">Type</span></span> | <span data-ttu-id="e1fe5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1fe5-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e1fe5-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1fe5-130">Authorization</span></span>  | <span data-ttu-id="e1fe5-131">string</span><span class="sxs-lookup"><span data-stu-id="e1fe5-131">string</span></span>  | <span data-ttu-id="e1fe5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e1fe5-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1fe5-134">Accept</span></span> | <span data-ttu-id="e1fe5-135">string</span><span class="sxs-lookup"><span data-stu-id="e1fe5-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="e1fe5-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fe5-136">Request body</span></span>
<span data-ttu-id="e1fe5-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1fe5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fe5-138">Response</span></span>

<span data-ttu-id="e1fe5-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e1fe5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1fe5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1fe5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1fe5-141">Request</span></span>
<span data-ttu-id="e1fe5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="e1fe5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1fe5-143">Response</span></span>
<span data-ttu-id="e1fe5-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1fe5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
