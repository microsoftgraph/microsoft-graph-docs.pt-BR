---
title: Obter onenoteOperation
description: 'Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.   '
localization_priority: Normal
ms.openlocfilehash: b62f83266560f217d9569c6ee7ca39dd53198bb7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824763"
---
# <a name="get-onenoteoperation"></a><span data-ttu-id="136d3-104">Obter onenoteOperation</span><span class="sxs-lookup"><span data-stu-id="136d3-104">Get onenoteOperation</span></span>

> <span data-ttu-id="136d3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="136d3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="136d3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="136d3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="136d3-p103">Obtenha o status de uma operação demorada do OneNote. Isso se aplica a operações que retornam o cabeçalho **Operation-Location** na resposta, como `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span><span class="sxs-lookup"><span data-stu-id="136d3-p103">Get the status of a long-running OneNote operation. This applies to operations that return the **Operation-Location** header in the response, such as `CopyNotebook`, `CopyToNotebook`, `CopyToSectionGroup`, `and CopyToSection`.</span></span>   

<span data-ttu-id="136d3-109">Você pode sondar o ponto de extremidade de Operation-Location até a propriedade `status` retornar `completed` ou `failed`.</span><span class="sxs-lookup"><span data-stu-id="136d3-109">You can poll the Operation-Location endpoint until the `status` property returns `completed` or `failed`.</span></span> 

<span data-ttu-id="136d3-110">Se o status for `completed`, a propriedade `resourceLocation` conterá o URI do ponto de extremidade do recurso.</span><span class="sxs-lookup"><span data-stu-id="136d3-110">If the status is `completed`, the `resourceLocation` property contains the resource endpoint URI.</span></span> 

<span data-ttu-id="136d3-111">Se o status for `failed`, o erro e as propriedades `@api.diagnostics` fornecerão informações de erro.</span><span class="sxs-lookup"><span data-stu-id="136d3-111">If the status is `failed`, the error and `@api.diagnostics` properties provide error information.</span></span>

## <a name="permissions"></a><span data-ttu-id="136d3-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="136d3-112">Permissions</span></span>
<span data-ttu-id="136d3-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="136d3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136d3-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="136d3-115">Permission type</span></span>      | <span data-ttu-id="136d3-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="136d3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="136d3-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="136d3-117">Delegated (work or school account)</span></span> | <span data-ttu-id="136d3-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136d3-118">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="136d3-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="136d3-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="136d3-120">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="136d3-120">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="136d3-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="136d3-121">Application</span></span> | <span data-ttu-id="136d3-122">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136d3-122">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="136d3-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="136d3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/operations/{id}
GET /users/{id | userPrincipalName}/onenote/operations/{id}
GET /groups/{id}/onenote/operations/{id}
GET /sites/{id}/onenote/operations/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="136d3-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="136d3-124">Optional query parameters</span></span>
<span data-ttu-id="136d3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="136d3-125">None.</span></span>

## <a name="request-headers"></a><span data-ttu-id="136d3-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="136d3-126">Request headers</span></span>
| <span data-ttu-id="136d3-127">Nome</span><span class="sxs-lookup"><span data-stu-id="136d3-127">Name</span></span>       | <span data-ttu-id="136d3-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="136d3-128">Type</span></span> | <span data-ttu-id="136d3-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="136d3-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="136d3-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="136d3-130">Authorization</span></span>  | <span data-ttu-id="136d3-131">string</span><span class="sxs-lookup"><span data-stu-id="136d3-131">string</span></span>  | <span data-ttu-id="136d3-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="136d3-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="136d3-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="136d3-134">Accept</span></span> | <span data-ttu-id="136d3-135">string</span><span class="sxs-lookup"><span data-stu-id="136d3-135">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="136d3-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="136d3-136">Request body</span></span>
<span data-ttu-id="136d3-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="136d3-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136d3-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="136d3-138">Response</span></span>

<span data-ttu-id="136d3-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [onenoteOperation](../resources/onenoteoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="136d3-139">If successful, this method returns a `200 OK` response code and [onenoteOperation](../resources/onenoteoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="136d3-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="136d3-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="136d3-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="136d3-141">Request</span></span>
<span data-ttu-id="136d3-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="136d3-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_onenoteoperation"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/operations/{id}
```
##### <a name="response"></a><span data-ttu-id="136d3-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="136d3-143">Response</span></span>
<span data-ttu-id="136d3-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="136d3-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
