---
title: Criar Sessão
description: 'Use essa API para criar uma nova sessão de pasta de trabalho. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ab4cc0d983efde535a4d92b6e918dfe9c9881170
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641859"
---
# <a name="create-session"></a><span data-ttu-id="42107-103">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="42107-103">Create Session</span></span>

<span data-ttu-id="42107-104">Use essa API para criar uma nova sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="42107-104">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="42107-105">As APIs do Excel podem ser chamadas em um destes dois modos:</span><span class="sxs-lookup"><span data-stu-id="42107-105">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="42107-p101">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação.</span><span class="sxs-lookup"><span data-stu-id="42107-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="42107-p102">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="42107-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="42107-112">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="42107-112">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="42107-p103">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="42107-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="42107-116">Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="42107-116">Error Handling</span></span>

<span data-ttu-id="42107-117">Essa solicitação poderá, ocasionalmente, receber uma mensagem de erro HTTP 504.</span><span class="sxs-lookup"><span data-stu-id="42107-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="42107-118">A resposta apropriada para esta mensagem de erro é repetir a solicitação.</span><span class="sxs-lookup"><span data-stu-id="42107-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="42107-119">Permissões</span><span class="sxs-lookup"><span data-stu-id="42107-119">Permissions</span></span>
<span data-ttu-id="42107-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42107-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42107-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42107-122">Permission type</span></span>      | <span data-ttu-id="42107-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42107-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42107-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42107-124">Delegated (work or school account)</span></span> | <span data-ttu-id="42107-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42107-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="42107-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42107-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42107-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42107-127">Not supported.</span></span>    |
|<span data-ttu-id="42107-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42107-128">Application</span></span> | <span data-ttu-id="42107-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42107-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42107-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42107-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="42107-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42107-131">Request headers</span></span>
| <span data-ttu-id="42107-132">Nome</span><span class="sxs-lookup"><span data-stu-id="42107-132">Name</span></span>       | <span data-ttu-id="42107-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="42107-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="42107-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="42107-134">Authorization</span></span>  | <span data-ttu-id="42107-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="42107-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="42107-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42107-137">Request body</span></span>
<span data-ttu-id="42107-138">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="42107-138">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="42107-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="42107-139">Response</span></span>

<span data-ttu-id="42107-140">Se for bem-sucedido, esse método retornará o código de resposta `201 Created` e o objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42107-140">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42107-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="42107-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="42107-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42107-142">Request</span></span>
<span data-ttu-id="42107-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="42107-143">Here is an example of the request.</span></span>
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
<span data-ttu-id="42107-144">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="42107-144">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="42107-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="42107-145">Response</span></span>
<span data-ttu-id="42107-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="42107-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

