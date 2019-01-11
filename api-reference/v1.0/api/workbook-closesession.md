---
title: Fechar Sessão
description: 'Use esta API para fechar uma sessão de pasta de trabalho existente. '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0e4d00b1ebf9ba90f6085f8dc7fc1005375efc0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818631"
---
# <a name="close-session"></a><span data-ttu-id="72e73-103">Fechar Sessão</span><span class="sxs-lookup"><span data-stu-id="72e73-103">Close Session</span></span>

<span data-ttu-id="72e73-104">Use esta API para fechar uma sessão de pasta de trabalho existente.</span><span class="sxs-lookup"><span data-stu-id="72e73-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="72e73-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72e73-105">Permissions</span></span>
<span data-ttu-id="72e73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72e73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72e73-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72e73-108">Permission type</span></span>      | <span data-ttu-id="72e73-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72e73-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72e73-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72e73-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72e73-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="72e73-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="72e73-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72e73-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72e73-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72e73-113">Not supported.</span></span>    |
|<span data-ttu-id="72e73-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72e73-114">Application</span></span> | <span data-ttu-id="72e73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72e73-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72e73-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72e73-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="72e73-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72e73-117">Request headers</span></span>
| <span data-ttu-id="72e73-118">Nome</span><span class="sxs-lookup"><span data-stu-id="72e73-118">Name</span></span>       | <span data-ttu-id="72e73-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="72e73-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72e73-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="72e73-120">Authorization</span></span>  | <span data-ttu-id="72e73-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72e73-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="72e73-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="72e73-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="72e73-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="72e73-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="72e73-126">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="72e73-126">workbook-session-id</span></span> | <span data-ttu-id="72e73-127">Id de sessão de pasta de trabalho a ser fechada</span><span class="sxs-lookup"><span data-stu-id="72e73-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="72e73-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72e73-128">Request body</span></span>
<span data-ttu-id="72e73-129">Esta API não exige o corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72e73-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="72e73-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="72e73-130">Response</span></span>

<span data-ttu-id="72e73-131">Se bem sucedido, este método retorna um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="72e73-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="72e73-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72e73-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72e73-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72e73-133">Request</span></span>
<span data-ttu-id="72e73-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72e73-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="72e73-135">Observe que o cabeçalho workbook-session-id é necessário.</span><span class="sxs-lookup"><span data-stu-id="72e73-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="72e73-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="72e73-136">Response</span></span>
<span data-ttu-id="72e73-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72e73-137">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
