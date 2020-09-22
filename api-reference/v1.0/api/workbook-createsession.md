---
title: 'Workbook: CreateSession'
description: Crie uma nova sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: a7b021173b28826642898d96c889a955f8bd182e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970898"
---
# <a name="workbook-createsession"></a><span data-ttu-id="11ef0-103">Workbook: CreateSession</span><span class="sxs-lookup"><span data-stu-id="11ef0-103">workbook: createSession</span></span>

<span data-ttu-id="11ef0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ef0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11ef0-105">Crie uma nova sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="11ef0-105">Create a new workbook session.</span></span> 

<span data-ttu-id="11ef0-106">As APIs do Excel podem ser chamadas em um destes dois modos:</span><span class="sxs-lookup"><span data-stu-id="11ef0-106">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="11ef0-p101">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação.</span><span class="sxs-lookup"><span data-stu-id="11ef0-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="11ef0-p102">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="11ef0-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="11ef0-113">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="11ef0-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="11ef0-p103">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="11ef0-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

<span data-ttu-id="11ef0-117">Em alguns casos, a criação de uma nova sessão requer um tempo indeterminado para ser concluída.</span><span class="sxs-lookup"><span data-stu-id="11ef0-117">In some cases, creating a new session requires an indeterminate time to complete.</span></span> <span data-ttu-id="11ef0-118">O Microsoft Graph também fornece um padrão de operações de longa duração.</span><span class="sxs-lookup"><span data-stu-id="11ef0-118">Microsoft Graph also provides a long running operations pattern.</span></span> <span data-ttu-id="11ef0-119">Este padrão oferece uma maneira de Pesquisar as atualizações de status de criação, sem esperar que a criação seja concluída.</span><span class="sxs-lookup"><span data-stu-id="11ef0-119">This pattern provides a way to poll for creation status updates, without waiting for the creation to complete.</span></span> <span data-ttu-id="11ef0-120">As etapas são as seguintes:</span><span class="sxs-lookup"><span data-stu-id="11ef0-120">The following are the steps:</span></span>

1. <span data-ttu-id="11ef0-121">Um `Prefer: respond-async` cabeçalho é adicionado à solicitação para indicar que se trata de uma operação de execução demorada.</span><span class="sxs-lookup"><span data-stu-id="11ef0-121">A `Prefer: respond-async` header is added to the request to indicate that it is a long-running operation.</span></span>
2. <span data-ttu-id="11ef0-122">A resposta retorna um `Location` cabeçalho para especificar a URL para sondar o status da operação de criação.</span><span class="sxs-lookup"><span data-stu-id="11ef0-122">The response returns a `Location` header to specify the URL for polling the creation operation status.</span></span> <span data-ttu-id="11ef0-123">Você pode obter o status da operação acessando a URL especificada.</span><span class="sxs-lookup"><span data-stu-id="11ef0-123">You can get the operation status by accessing the specified URL.</span></span> <span data-ttu-id="11ef0-124">O status será um dos seguintes: `notStarted` , `running` , `succeeded` ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="11ef0-124">The status will be one of the following: `notStarted`, `running`, `succeeded`, or `failed`.</span></span>
3. <span data-ttu-id="11ef0-125">Após a conclusão da operação, você pode solicitar o status novamente e a resposta mostrará `succeeded` ou `failed` .</span><span class="sxs-lookup"><span data-stu-id="11ef0-125">After the operation completes, you can request the status again and the response will show either `succeeded` or `failed`.</span></span>

## <a name="error-handling"></a><span data-ttu-id="11ef0-126">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="11ef0-126">Error handling</span></span>

<span data-ttu-id="11ef0-127">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="11ef0-127">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="11ef0-128">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="11ef0-128">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="11ef0-129">Permissões</span><span class="sxs-lookup"><span data-stu-id="11ef0-129">Permissions</span></span>
<span data-ttu-id="11ef0-p107">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11ef0-p107">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11ef0-132">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11ef0-132">Permission type</span></span>      | <span data-ttu-id="11ef0-133">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11ef0-133">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11ef0-134">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11ef0-134">Delegated (work or school account)</span></span> | <span data-ttu-id="11ef0-135">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11ef0-135">Files.ReadWrite</span></span>    |
|<span data-ttu-id="11ef0-136">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11ef0-136">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11ef0-137">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11ef0-137">Not supported.</span></span>    |
|<span data-ttu-id="11ef0-138">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11ef0-138">Application</span></span> | <span data-ttu-id="11ef0-139">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11ef0-139">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11ef0-140">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11ef0-140">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession
```
## <a name="request-headers"></a><span data-ttu-id="11ef0-141">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11ef0-141">Request headers</span></span>
| <span data-ttu-id="11ef0-142">Nome</span><span class="sxs-lookup"><span data-stu-id="11ef0-142">Name</span></span>       | <span data-ttu-id="11ef0-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="11ef0-143">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="11ef0-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="11ef0-144">Authorization</span></span>  | <span data-ttu-id="11ef0-p108">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="11ef0-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11ef0-147">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11ef0-147">Request body</span></span>
<span data-ttu-id="11ef0-148">No corpo da solicitação, forneça uma representação JSON do objeto [workbookSessionInfo](../resources/workbooksessioninfo.md) .</span><span class="sxs-lookup"><span data-stu-id="11ef0-148">In the request body, supply a JSON representation of [workbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11ef0-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="11ef0-149">Response</span></span>

<span data-ttu-id="11ef0-150">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [workbookSessionInfo](../resources/workbooksessioninfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11ef0-150">If successful, this method returns a `201 Created` response code and a [workbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span> <span data-ttu-id="11ef0-151">Para uma operação de execução longa, ele retorna um `202 Accepted ` código de resposta e um `Location` cabeçalho com um corpo vazio na resposta.</span><span class="sxs-lookup"><span data-stu-id="11ef0-151">For a long-running operation, it returns a `202 Accepted ` response code and a `Location` header with an empty body in the response.</span></span>

## <a name="examples"></a><span data-ttu-id="11ef0-152">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11ef0-152">Examples</span></span>

### <a name="example-1-basic-session-creation"></a><span data-ttu-id="11ef0-153">Exemplo 1: criação de sessão básica</span><span class="sxs-lookup"><span data-stu-id="11ef0-153">Example 1: Basic session creation</span></span>
#### <a name="request"></a><span data-ttu-id="11ef0-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11ef0-154">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="11ef0-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="11ef0-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
# <a name="c"></a>[<span data-ttu-id="11ef0-156">C#</span><span class="sxs-lookup"><span data-stu-id="11ef0-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-excel-session-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11ef0-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11ef0-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-excel-session-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11ef0-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11ef0-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-excel-session-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11ef0-159">Java</span><span class="sxs-lookup"><span data-stu-id="11ef0-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-excel-session-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="11ef0-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="11ef0-160">Response</span></span>
><span data-ttu-id="11ef0-161">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11ef0-161">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-session-creation-with-long-running-operation-pattern"></a><span data-ttu-id="11ef0-162">Exemplo 2: criação de sessão com um padrão de operação de execução longa</span><span class="sxs-lookup"><span data-stu-id="11ef0-162">Example 2: Session creation with long-running operation pattern</span></span>

#### <a name="request"></a><span data-ttu-id="11ef0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11ef0-163">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

#### <a name="response"></a><span data-ttu-id="11ef0-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="11ef0-164">Response</span></span>
><span data-ttu-id="11ef0-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="11ef0-165">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json
{
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

