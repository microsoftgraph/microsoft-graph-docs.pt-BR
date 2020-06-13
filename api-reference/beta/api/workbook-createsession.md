---
title: Criar Sessão
description: 'Use essa API para criar uma nova sessão de pasta de trabalho. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 33a52d7ce90d7fcd7ea8c20464c81a2d3c907348
ms.sourcegitcommit: d6374f42bee4de11fd7a3d0d8c2a7f8c4e7739bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2020
ms.locfileid: "44710668"
---
# <a name="create-session"></a><span data-ttu-id="9e155-103">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="9e155-103">Create Session</span></span>

<span data-ttu-id="9e155-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e155-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e155-105">Use essa API para criar uma nova sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9e155-105">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="9e155-106">As APIs do Excel podem ser chamadas em um destes dois modos:</span><span class="sxs-lookup"><span data-stu-id="9e155-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="9e155-p101">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação.</span><span class="sxs-lookup"><span data-stu-id="9e155-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="9e155-p102">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="9e155-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="9e155-113">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="9e155-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="9e155-p103">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="9e155-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="9e155-117">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="9e155-117">Error Handling</span></span>

<span data-ttu-id="9e155-118">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="9e155-118">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="9e155-119">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e155-119">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e155-120">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e155-120">Permissions</span></span>
<span data-ttu-id="9e155-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e155-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e155-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e155-123">Permission type</span></span>      | <span data-ttu-id="9e155-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e155-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e155-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e155-125">Delegated (work or school account)</span></span> | <span data-ttu-id="9e155-126">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9e155-126">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9e155-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e155-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e155-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e155-128">Not supported.</span></span>    |
|<span data-ttu-id="9e155-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e155-129">Application</span></span> | <span data-ttu-id="9e155-130">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e155-130">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e155-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e155-131">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession
```
## <a name="request-headers"></a><span data-ttu-id="9e155-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e155-132">Request headers</span></span>
| <span data-ttu-id="9e155-133">Nome</span><span class="sxs-lookup"><span data-stu-id="9e155-133">Name</span></span>       | <span data-ttu-id="9e155-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e155-134">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e155-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="9e155-135">Authorization</span></span>  | <span data-ttu-id="9e155-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9e155-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e155-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e155-138">Request body</span></span>
<span data-ttu-id="9e155-139">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md) .</span><span class="sxs-lookup"><span data-stu-id="9e155-139">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9e155-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e155-140">Response</span></span>

<span data-ttu-id="9e155-141">Se bem-sucedido, este método retorna o `201 Created` código de resposta e o objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e155-141">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e155-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e155-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e155-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e155-143">Request</span></span>
<span data-ttu-id="9e155-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e155-144">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e155-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e155-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[<span data-ttu-id="9e155-146">C#</span><span class="sxs-lookup"><span data-stu-id="9e155-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e155-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e155-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e155-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e155-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="9e155-149">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md) .</span><span class="sxs-lookup"><span data-stu-id="9e155-149">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="9e155-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e155-150">Response</span></span>
<span data-ttu-id="9e155-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e155-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
