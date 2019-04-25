---
title: Fechar sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ff089565cc885cc5d70fbea238335b546b41f2ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547610"
---
# <a name="close-session"></a><span data-ttu-id="bc5e6-103">Fechar sessão</span><span class="sxs-lookup"><span data-stu-id="bc5e6-103">Close Session</span></span>

<span data-ttu-id="bc5e6-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bc5e6-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bc5e6-105">Permissions</span></span>
<span data-ttu-id="bc5e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc5e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc5e6-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bc5e6-108">Permission type</span></span>      | <span data-ttu-id="bc5e6-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bc5e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc5e6-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bc5e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc5e6-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc5e6-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="bc5e6-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bc5e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc5e6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-113">Not supported.</span></span>    |
|<span data-ttu-id="bc5e6-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bc5e6-114">Application</span></span> | <span data-ttu-id="bc5e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc5e6-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bc5e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="bc5e6-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5e6-117">Request headers</span></span>
| <span data-ttu-id="bc5e6-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bc5e6-118">Name</span></span>       | <span data-ttu-id="bc5e6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc5e6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bc5e6-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bc5e6-120">Authorization</span></span>  | <span data-ttu-id="bc5e6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc5e6-123">Workbook-session-ID</span><span class="sxs-lookup"><span data-stu-id="bc5e6-123">workbook-session-id</span></span> | <span data-ttu-id="bc5e6-124">ID da sessão da pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="bc5e6-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc5e6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5e6-125">Request body</span></span>
<span data-ttu-id="bc5e6-126">Essa API não requer nenhum corpo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="bc5e6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5e6-127">Response</span></span>

<span data-ttu-id="bc5e6-128">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bc5e6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bc5e6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc5e6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bc5e6-130">Request</span></span>
<span data-ttu-id="bc5e6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="bc5e6-132">Observe que o cabeçalho Workbook-session-ID é necessário.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="bc5e6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bc5e6-133">Response</span></span>
<span data-ttu-id="bc5e6-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bc5e6-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
