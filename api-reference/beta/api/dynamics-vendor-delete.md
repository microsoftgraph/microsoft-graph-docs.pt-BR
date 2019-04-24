---
title: Excluir fornecedores
description: Exclui um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: e9ef641d8c1d6995e93eaaf87a7131e246c9a0f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458625"
---
# <a name="delete-vendors"></a><span data-ttu-id="607ef-103">Excluir fornecedores</span><span class="sxs-lookup"><span data-stu-id="607ef-103">Delete vendors</span></span>
<span data-ttu-id="607ef-104">Excluir um objeto fornecedor do Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="607ef-104">Delete a vendor object from Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="607ef-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="607ef-105">Permissions</span></span>
<span data-ttu-id="607ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607ef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="607ef-108">Permission type</span></span> |<span data-ttu-id="607ef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="607ef-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="607ef-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="607ef-110">Delegated (work or school account)</span></span>|<span data-ttu-id="607ef-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607ef-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="607ef-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="607ef-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="607ef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="607ef-113">Not supported.</span></span>|
|<span data-ttu-id="607ef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="607ef-114">Application</span></span>|<span data-ttu-id="607ef-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607ef-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="607ef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="607ef-116">HTTP request</span></span>
```
DELETE /financials/companies('{id}')/vendors('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="607ef-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="607ef-117">Optional query parameters</span></span>
<span data-ttu-id="607ef-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="607ef-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="607ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="607ef-119">Request headers</span></span>
|<span data-ttu-id="607ef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="607ef-120">Header</span></span>|<span data-ttu-id="607ef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="607ef-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="607ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="607ef-122">Authorization</span></span>  |<span data-ttu-id="607ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607ef-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="607ef-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="607ef-125">If-Match</span></span>       |<span data-ttu-id="607ef-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="607ef-126">Required.</span></span> <span data-ttu-id="607ef-127">Quando esse cabeçalho de solicitação for incluído e a eTag fornecida não corresponder à marca atual nos **fornecedores**, os **fornecedores** não serão atualizados.</span><span class="sxs-lookup"><span data-stu-id="607ef-127">When this request header is included and the eTag provided does not match the current tag on the **vendors**, the **vendors** will not be updated.</span></span> |

## <a name="request-body"></a><span data-ttu-id="607ef-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="607ef-128">Request body</span></span>
<span data-ttu-id="607ef-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="607ef-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="607ef-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="607ef-130">Response</span></span>
<span data-ttu-id="607ef-p104">Se bem-sucedido, este método retorna um código de resposta ```204 No Content```. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607ef-p104">If successful, this method returns ```204 No Content``` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="607ef-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="607ef-133">Example</span></span>

<span data-ttu-id="607ef-134">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="607ef-134">**Request**</span></span>

<span data-ttu-id="607ef-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="607ef-135">Here is an example of the request.</span></span>

```json
DELETE https://graph.microsoft.com/beta/financials/companies('{id}')/vendors('{id}')
```

<span data-ttu-id="607ef-136">**Response**</span><span class="sxs-lookup"><span data-stu-id="607ef-136">**Response**</span></span> 

<span data-ttu-id="607ef-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="607ef-137">Here is an example of the response.</span></span> 

```json
HTTP/1.1 204 No Content
```
