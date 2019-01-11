---
title: Atualizar Sessão
description: 'Use esta API para atualizar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2f4d454214d2f21d1f6447ee224f3013cebb9078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822334"
---
# <a name="refresh-session"></a><span data-ttu-id="fd993-103">Atualizar Sessão</span><span class="sxs-lookup"><span data-stu-id="fd993-103">Refresh Session</span></span>

<span data-ttu-id="fd993-104">Use esta API para atualizar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="fd993-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fd993-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd993-105">Permissions</span></span>
<span data-ttu-id="fd993-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd993-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd993-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd993-108">Permission type</span></span>      | <span data-ttu-id="fd993-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd993-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd993-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd993-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd993-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd993-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="fd993-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd993-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd993-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd993-113">Not supported.</span></span>    |
|<span data-ttu-id="fd993-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd993-114">Application</span></span> | <span data-ttu-id="fd993-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fd993-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd993-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd993-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="fd993-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd993-117">Request headers</span></span>
| <span data-ttu-id="fd993-118">Nome</span><span class="sxs-lookup"><span data-stu-id="fd993-118">Name</span></span>       | <span data-ttu-id="fd993-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd993-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd993-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd993-120">Authorization</span></span>  | <span data-ttu-id="fd993-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd993-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fd993-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="fd993-123">workbook-session-id</span></span> | <span data-ttu-id="fd993-124">ID de sessão da pasta de trabalho que será atualizada</span><span class="sxs-lookup"><span data-stu-id="fd993-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd993-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd993-125">Request body</span></span>
<span data-ttu-id="fd993-126">Esta API não exige o corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd993-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="fd993-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd993-127">Response</span></span>

<span data-ttu-id="fd993-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fd993-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd993-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd993-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd993-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fd993-130">Request</span></span>
<span data-ttu-id="fd993-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fd993-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="fd993-132">Observe que o cabeçalho workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="fd993-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="fd993-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd993-133">Response</span></span>
<span data-ttu-id="fd993-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fd993-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
