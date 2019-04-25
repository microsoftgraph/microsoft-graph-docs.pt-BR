---
title: Atualizar sessão
description: 'Use esta API para atualizar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: c10372e332072eb69bfb605484695d950185e62c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534693"
---
# <a name="refresh-session"></a><span data-ttu-id="bbfce-103">Atualizar sessão</span><span class="sxs-lookup"><span data-stu-id="bbfce-103">Refresh Session</span></span>

<span data-ttu-id="bbfce-104">Use esta API para atualizar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="bbfce-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bbfce-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bbfce-105">Permissions</span></span>
<span data-ttu-id="bbfce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbfce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbfce-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbfce-108">Permission type</span></span>      | <span data-ttu-id="bbfce-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bbfce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bbfce-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbfce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bbfce-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bbfce-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bbfce-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbfce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bbfce-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbfce-113">Not supported.</span></span>    |
|<span data-ttu-id="bbfce-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbfce-114">Application</span></span> | <span data-ttu-id="bbfce-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbfce-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bbfce-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbfce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="bbfce-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfce-117">Request headers</span></span>
| <span data-ttu-id="bbfce-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bbfce-118">Name</span></span>       | <span data-ttu-id="bbfce-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbfce-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bbfce-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbfce-120">Authorization</span></span>  | <span data-ttu-id="bbfce-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbfce-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bbfce-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="bbfce-123">workbook-session-id</span></span> | <span data-ttu-id="bbfce-124">ID da sessão da pasta de trabalho a ser atualizada</span><span class="sxs-lookup"><span data-stu-id="bbfce-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="bbfce-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfce-125">Request body</span></span>
<span data-ttu-id="bbfce-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbfce-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="bbfce-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfce-127">Response</span></span>

<span data-ttu-id="bbfce-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bbfce-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bbfce-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbfce-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bbfce-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbfce-130">Request</span></span>
<span data-ttu-id="bbfce-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbfce-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="bbfce-132">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="bbfce-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="bbfce-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbfce-133">Response</span></span>
<span data-ttu-id="bbfce-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbfce-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
