---
title: Práticas recomendadas para APIs do Excel no Microsoft Graph
description: Listar as práticas recomendadas e exemplos para as APIs do Excel no Microsoft Graph
author: grangeryy
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d824cf89a07c81bae3a2e129896da9af282be49c
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598567"
---
# <a name="best-practices-for-working-with-the-excel-api-in-microsoft-graph"></a><span data-ttu-id="f3ef2-103">Práticas recomendadas para trabalhar com a API do Excel no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f3ef2-103">Best practices for working with the Excel API in Microsoft Graph</span></span>

<span data-ttu-id="f3ef2-104">Este artigo fornece recomendações para trabalhar com as APIs do Excel no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-104">This article provides recommendations for working with the Excel APIs in Microsoft Graph.</span></span>

## <a name="manage-sessions-in-the-most-efficient-way"></a><span data-ttu-id="f3ef2-105">Gerenciar sessões da maneira mais eficiente</span><span class="sxs-lookup"><span data-stu-id="f3ef2-105">Manage sessions in the most efficient way</span></span>

<span data-ttu-id="f3ef2-106">Se você tiver mais de uma chamada para fazer dentro de um determinado período de tempo, recomendamos que você crie uma sessão e passe a ID da sessão com cada solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-106">If you have more than one call to make within a certain period of time, we recommend that you create a session and pass the session ID with each request.</span></span> <span data-ttu-id="f3ef2-107">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-107">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> <span data-ttu-id="f3ef2-108">Fazendo isso, você pode usar as APIs do Excel da maneira mais eficiente.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-108">By doing so, you can use the Excel APIs in the most efficient way.</span></span>

<span data-ttu-id="f3ef2-109">O exemplo a seguir mostra como adicionar um novo número a uma tabela e localizar um registro em uma pasta de trabalho usando essa abordagem.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-109">The following example shows you how to add a new number to a table and then find one record in a workbook using this approach.</span></span>

### <a name="step-1-create-a-session"></a><span data-ttu-id="f3ef2-110">Etapa 1: criar uma sessão</span><span class="sxs-lookup"><span data-stu-id="f3ef2-110">Step 1: Create a session</span></span>

#### <a name="request"></a><span data-ttu-id="f3ef2-111">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ef2-111">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
#### <a name="response"></a><span data-ttu-id="f3ef2-112">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ef2-112">Response</span></span>

<span data-ttu-id="f3ef2-113">A seguir está uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-113">The following is a successful response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

### <a name="step-2-add-a-new-row-to-the-table"></a><span data-ttu-id="f3ef2-114">Etapa 2: adicionar uma nova linha à tabela</span><span class="sxs-lookup"><span data-stu-id="f3ef2-114">Step 2: Add a new row to the table</span></span>

#### <a name="request"></a><span data-ttu-id="f3ef2-115">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ef2-115">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/Table1/rows/add
Content-type: application/json
workbook-session-id: {session-id}

{
  "values": [[“east”, “pear”, 4]]
}
```

#### <a name="response"></a><span data-ttu-id="f3ef2-116">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ef2-116">Response</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 42

{
  "index": 6,
  "values": [[“east”, “pear”, 4]]
}
```

### <a name="step-3-look-up-a-value-in-the-updated-table"></a><span data-ttu-id="f3ef2-117">Etapa 3: Pesquisar um valor na tabela atualizada</span><span class="sxs-lookup"><span data-stu-id="f3ef2-117">Step 3: Look up a value in the updated table</span></span>

#### <a name="request"></a><span data-ttu-id="f3ef2-118">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ef2-118">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/functions/vlookup
Content-type: application/json
workbook-session-id: {session-id}

{
    "lookupValue":"pear",
    "tableArray":{"Address":"Sheet1!B2:C7"},
    "colIndexNum":2,
    "rangeLookup":false
}
```

#### <a name="response"></a><span data-ttu-id="f3ef2-119">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ef2-119">Response</span></span>

```http
HTTP code: 200 OK
content-type: application/json

{
    "value": 5
}
```

### <a name="step-4-close-the-session-after-all-the-requests-are-completed"></a><span data-ttu-id="f3ef2-120">Etapa 4: fechar a sessão após todas as solicitações serem concluídas</span><span class="sxs-lookup"><span data-stu-id="f3ef2-120">Step 4: Close the session after all the requests are completed</span></span>

#### <a name="request"></a><span data-ttu-id="f3ef2-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3ef2-121">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{
}
```

#### <a name="response"></a><span data-ttu-id="f3ef2-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ef2-122">Response</span></span>

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="f3ef2-123">Para obter mais detalhes, consulte [criar sessão](/graph/api/workbook-createsession?view=graph-rest-1.0) e [fechar sessão](/graph/api/workbook-closesession?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f3ef2-123">For more details, see [Create session](/graph/api/workbook-createsession?view=graph-rest-1.0) and [Close session](/graph/api/workbook-closesession?view=graph-rest-1.0).</span></span>

## <a name="working-with-apis-that-take-a-long-time-to-complete"></a><span data-ttu-id="f3ef2-124">Trabalhar com APIs que levar muito tempo para ser concluído</span><span class="sxs-lookup"><span data-stu-id="f3ef2-124">Working with APIs that take a long time to complete</span></span>

<span data-ttu-id="f3ef2-125">Você pode notar que algumas operações levam um tempo indeterminado para a conclusão; por exemplo, abrir uma pasta de trabalho grande.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-125">You might notice that some operations take an indeterminate amount time to complete; for example, opening a large workbook.</span></span> <span data-ttu-id="f3ef2-126">É fácil atingir o tempo limite enquanto aguarda a resposta para essas solicitações.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-126">It is easy to hit timeout while waiting for the response to these requests.</span></span> <span data-ttu-id="f3ef2-127">Para resolver esse problema, fornecemos o padrão de operação de longa execução.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-127">To resolve this issue, we provide the long-running operation pattern.</span></span> <span data-ttu-id="f3ef2-128">Ao usar esse padrão, você não precisa se preocupar com o tempo limite da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-128">When you use this pattern, you don't need to worry about the timeout for the request.</span></span>

<span data-ttu-id="f3ef2-129">Atualmente, a API do Excel de criação de sessão no Microsoft Graph tem o padrão de operação de execução demorada habilitado.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-129">Currently, the session creation Excel API in Microsoft Graph has the long-running operation pattern enabled.</span></span> <span data-ttu-id="f3ef2-130">Este padrão envolve as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="f3ef2-130">This pattern involves the following steps:</span></span>

1. <span data-ttu-id="f3ef2-131">Adicione um `Prefer: respond-async` cabeçalho à solicitação para indicar que é uma operação de execução demorada quando você faz uma sessão.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-131">Add a `Prefer: respond-async` header to the request to indicate that it is a long-running operation when you crate a session.</span></span>
2. <span data-ttu-id="f3ef2-132">Uma operação de execução longa retornará uma `202 Accepted` resposta junto com um cabeçalho de local para recuperar o status da operação.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-132">A long-running operation will return a `202 Accepted` response along with a Location header to retrieve the operation status.</span></span> <span data-ttu-id="f3ef2-133">Se a criação da sessão for concluída em vários segundos, ela retornará uma resposta de criação de sessão regular em vez de usar o padrão de operação de longa execução.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-133">If the session creation completes in several seconds, it will return a regular create session response instead of using the long-running operation pattern.</span></span>
3. <span data-ttu-id="f3ef2-134">Com a `202 Accepted` resposta, você pode recuperar o status da operação no local especificado.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-134">With the `202 Accepted` response, you can retrieve the operation status at the specified location.</span></span> <span data-ttu-id="f3ef2-135">Os valores de status de operação incluem `notStarted` ,, `running` `succeeded` e `failed` .</span><span class="sxs-lookup"><span data-stu-id="f3ef2-135">Operation status values include `notStarted`, `running`, `succeeded`, and `failed`.</span></span>
4. <span data-ttu-id="f3ef2-136">Após a conclusão da operação, você pode obter o resultado da criação da sessão através da URL especificada na resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-136">After the operation completes, you can get the session creation result through the specified URL in the succeeded response.</span></span>

<span data-ttu-id="f3ef2-137">O exemplo a seguir cria uma sessão usando o padrão de operação de longa execução.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-137">The following example creates a session using the long-running operation pattern.</span></span>

### <a name="initial-request-to-create-session"></a><span data-ttu-id="f3ef2-138">Solicitação inicial para criar sessão</span><span class="sxs-lookup"><span data-stu-id="f3ef2-138">Initial request to create session</span></span>

```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/worksheets({id})/createSession
Prefer: respond-async
Content-type: application/json
{
    "persistChanges": true
}
```

### <a name="response"></a><span data-ttu-id="f3ef2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3ef2-139">Response</span></span>

<span data-ttu-id="f3ef2-140">O padrão de operação de execução longa retornará uma `202 Accepted` resposta semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-140">The long-running operation pattern will return a `202 Accepted` response similar to the following.</span></span>

```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
Content-type: application/json

{
}
```

<span data-ttu-id="f3ef2-141">Em alguns casos, se a criação for bem-sucedida em segundos, ela não irá inserir o padrão de operação de longa execução; em vez disso, ele retorna como uma sessão de criação regular e a solicitação bem-sucedida retornará uma `201 Created` resposta.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-141">In some cases, if the creation succeeds within seconds, it won't enter the long-running operation pattern; instead, it returns as a regular create session and the successful request will return a `201 Created` response.</span></span>

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

<span data-ttu-id="f3ef2-142">O exemplo a seguir mostra a resposta quando a solicitação falha.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-142">The following example shows the response when the request fails.</span></span>

><span data-ttu-id="f3ef2-143">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-143">**Note:** The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 500 Internal Server Error
Content-type: application/json
{
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}


### Poll status of the long-running create session

With the long-running operation pattern, you can get the creation status at specified location by using the following request. The suggested interval to poll status is around 30 seconds. The maximum interval should be no more than 4 minutes.

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}
{
}
```

<span data-ttu-id="f3ef2-144">A seguir está a resposta quando a operação tem um status de `running` .</span><span class="sxs-lookup"><span data-stu-id="f3ef2-144">The following is the response when the operation has a status of `running`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": {operation-id},
    "status": "running"
}
```

<span data-ttu-id="f3ef2-145">A seguir está a resposta quando o status da operação é `succeeded` .</span><span class="sxs-lookup"><span data-stu-id="f3ef2-145">The following is the response when the operation status is `succeeded`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": {operation-id},
    "status": "succeeded",
    "resourceLocation": "https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
}
```

<span data-ttu-id="f3ef2-146">A seguir está a resposta quando o status da operação é `failed` .</span><span class="sxs-lookup"><span data-stu-id="f3ef2-146">The following is the response when the operation status is `failed`.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
  "id": {operation-id},
  "status": "failed",
  "error":{
    "code": "internalServerError",
    "message": "An internal server error occurred while processing the request.",
    "innerError": {
      "code": ""internalServerErrorUncategorized",
      "message": "An unspecified error has occurred.",
      "innerError": {
        "code": "GenericFileOpenError",
        "message": "The workbook cannot be opened."
      }
    }
  }
}
```

<span data-ttu-id="f3ef2-147">Para obter mais detalhes sobre erros, consulte [códigos de erro](/concepts/workbook-error-codes.md)</span><span class="sxs-lookup"><span data-stu-id="f3ef2-147">For more details about errors, see [Error codes](/concepts/workbook-error-codes.md)</span></span>

### <a name="acquire-session-information"></a><span data-ttu-id="f3ef2-148">Obter informações de sessão</span><span class="sxs-lookup"><span data-stu-id="f3ef2-148">Acquire session information</span></span>

<span data-ttu-id="f3ef2-149">Com o status de `succeeded` , você pode obter as informações da sessão criada por meio de `resourceLocation` uma solicitação semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-149">With a status of `succeeded`, you can get the created session information through `resourceLocation` with a request similar to the following.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{drive-item-id}/workbook/sessionInfoResource(key='{key}')
{
}
```

<span data-ttu-id="f3ef2-150">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-150">The following is the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "id": "id-value",
    "persistChanges": true
}
```

><span data-ttu-id="f3ef2-151">**Observação:** Obter informações de sessão depende da solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-151">**Note:** Acquire session information depends on the initial request.</span></span> <span data-ttu-id="f3ef2-152">Você não precisará adquirir o resultado se a solicitação inicial não retornar um corpo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f3ef2-152">You don't need to acquire the result if the initial request doesn't return a response body.</span></span>
