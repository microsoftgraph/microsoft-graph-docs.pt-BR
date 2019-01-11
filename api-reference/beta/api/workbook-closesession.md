---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: b9caf1a6b055522966ff35c8c1726642d57df262
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883668"
---
# <a name="close-session"></a><span data-ttu-id="ccca0-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="ccca0-103">Close Session</span></span>

<span data-ttu-id="ccca0-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="ccca0-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ccca0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccca0-105">Permissions</span></span>
<span data-ttu-id="ccca0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccca0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccca0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccca0-108">Permission type</span></span>      | <span data-ttu-id="ccca0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccca0-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ccca0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccca0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ccca0-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ccca0-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="ccca0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccca0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccca0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccca0-113">Not supported.</span></span>    |
|<span data-ttu-id="ccca0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccca0-114">Application</span></span> | <span data-ttu-id="ccca0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccca0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccca0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccca0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="ccca0-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccca0-117">Request headers</span></span>
| <span data-ttu-id="ccca0-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ccca0-118">Name</span></span>       | <span data-ttu-id="ccca0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccca0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ccca0-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccca0-120">Authorization</span></span>  | <span data-ttu-id="ccca0-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccca0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ccca0-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="ccca0-123">workbook-session-id</span></span> | <span data-ttu-id="ccca0-124">Id de sessão de pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="ccca0-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="ccca0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccca0-125">Request body</span></span>
<span data-ttu-id="ccca0-126">Esta API não exige o corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccca0-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="ccca0-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccca0-127">Response</span></span>

<span data-ttu-id="ccca0-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ccca0-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ccca0-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ccca0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ccca0-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccca0-130">Request</span></span>
<span data-ttu-id="ccca0-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccca0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="ccca0-132">Observe que o cabeçalho workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="ccca0-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="ccca0-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccca0-133">Response</span></span>
<span data-ttu-id="ccca0-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccca0-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
