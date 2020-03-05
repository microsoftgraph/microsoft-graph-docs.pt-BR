---
title: Excluir journalLines
description: Exclui uma linha de diário no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 64de86b424bed9a1592ceb7ae5194c42d9233352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42428926"
---
# <a name="delete-journallines"></a><span data-ttu-id="1c277-103">Excluir journalLines</span><span class="sxs-lookup"><span data-stu-id="1c277-103">Delete journalLines</span></span>

<span data-ttu-id="1c277-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1c277-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c277-105">Excluir um objeto de linha do diário do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="1c277-105">Delete a journal line object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c277-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1c277-106">Permissions</span></span>
<span data-ttu-id="1c277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c277-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1c277-109">Permission type</span></span> |<span data-ttu-id="1c277-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1c277-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="1c277-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1c277-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c277-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c277-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="1c277-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1c277-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="1c277-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1c277-114">Not supported.</span></span>|
|<span data-ttu-id="1c277-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1c277-115">Application</span></span>|<span data-ttu-id="1c277-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c277-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c277-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1c277-117">HTTP request</span></span>
```
DELETE /financials/companies/{id}/journals/{id}/journalLines/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c277-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1c277-118">Optional query parameters</span></span>
<span data-ttu-id="1c277-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1c277-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c277-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1c277-120">Request headers</span></span>
|<span data-ttu-id="1c277-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1c277-121">Header</span></span>          |<span data-ttu-id="1c277-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1c277-122">Value</span></span>                     |
|----------------|--------------------------|
|<span data-ttu-id="1c277-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1c277-123">Authorization</span></span>   |<span data-ttu-id="1c277-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c277-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="1c277-126">If-Match</span><span class="sxs-lookup"><span data-stu-id="1c277-126">If-Match</span></span>        |<span data-ttu-id="1c277-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1c277-127">Required.</span></span> <span data-ttu-id="1c277-128">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual no **journalLines**, o **journalLines** não será atualizado.</span><span class="sxs-lookup"><span data-stu-id="1c277-128">When this request header is included and the eTag provided does not match the current tag on the **journalLines**, the **journalLines** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c277-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1c277-129">Request body</span></span>

<span data-ttu-id="1c277-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1c277-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c277-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1c277-131">Response</span></span>

<span data-ttu-id="1c277-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c277-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c277-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1c277-134">Example</span></span>

<span data-ttu-id="1c277-135">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1c277-135">**Request**</span></span>

<span data-ttu-id="1c277-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1c277-136">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies/{id}/journals/{id}/journalLines/{id}
```

<span data-ttu-id="1c277-137">**Response**</span><span class="sxs-lookup"><span data-stu-id="1c277-137">**Response**</span></span> 

<span data-ttu-id="1c277-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1c277-138">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
