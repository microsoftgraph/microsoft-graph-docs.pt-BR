---
title: Criar categorias de categoria
description: Cria um objeto de categoria de item no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 6d3e2918854e169c13971d0c71fc66091874d3ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463730"
---
# <a name="create-itemcategories"></a><span data-ttu-id="c3fcb-103">Criar categorias de categoria</span><span class="sxs-lookup"><span data-stu-id="c3fcb-103">Create itemCategories</span></span>
<span data-ttu-id="c3fcb-104">Criar um objeto de categoria de item Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-104">Create an item category object Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3fcb-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3fcb-105">Permissions</span></span>
<span data-ttu-id="c3fcb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3fcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3fcb-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3fcb-108">Permission type</span></span> |<span data-ttu-id="c3fcb-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3fcb-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="c3fcb-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3fcb-110">Delegated (work or school account)</span></span>|<span data-ttu-id="c3fcb-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3fcb-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="c3fcb-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="c3fcb-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c3fcb-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-113">Not supported.</span></span>|
|<span data-ttu-id="c3fcb-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3fcb-114">Application</span></span>|<span data-ttu-id="c3fcb-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3fcb-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3fcb-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3fcb-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/itemCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3fcb-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c3fcb-117">Optional query parameters</span></span>
<span data-ttu-id="c3fcb-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3fcb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3fcb-119">Request headers</span></span>
|<span data-ttu-id="c3fcb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3fcb-120">Header</span></span>       |<span data-ttu-id="c3fcb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c3fcb-121">Value</span></span>                    |
|-------------|-------------------------|
|<span data-ttu-id="c3fcb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3fcb-122">Authorization</span></span>|<span data-ttu-id="c3fcb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3fcb-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c3fcb-125">Content-Type</span></span> |<span data-ttu-id="c3fcb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3fcb-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="c3fcb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3fcb-127">Request body</span></span>
<span data-ttu-id="c3fcb-128">No corpo da solicitação, forneça uma representação JSON de um \*\*\*\* objeto myCategories.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-128">In the request body, supply a JSON representation of an **itemCategories** object.</span></span>

## <a name="response"></a><span data-ttu-id="c3fcb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3fcb-129">Response</span></span>
<span data-ttu-id="c3fcb-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto myCategories no corpo da resposta. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="c3fcb-130">If successful, this method returns ```201 Created``` response code and an **itemCategories** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3fcb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3fcb-131">Example</span></span>

<span data-ttu-id="c3fcb-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="c3fcb-132">**Request**</span></span>

<span data-ttu-id="c3fcb-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/itemCategories
Content-type: application/json

{
  "code": "CHAIR",
  "displayName": "Office Chair"
}
```

<span data-ttu-id="c3fcb-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="c3fcb-134">**Response**</span></span>

<span data-ttu-id="c3fcb-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="c3fcb-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c3fcb-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3fcb-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "CHAIR",
  "displayName": "Office Chair",
  "lastModifiedDateTime": "2017-03-15T02:21:24.047Z"
}

```




