---
title: Criar countriesRegions
description: Cria um objeto de países/regiões no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a78ba9ce04dc1b9a5a39cf9e742de7503afc9c3f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454129"
---
# <a name="create-countriesregions"></a><span data-ttu-id="aa29a-103">Criar countriesRegions</span><span class="sxs-lookup"><span data-stu-id="aa29a-103">Create countriesRegions</span></span>
<span data-ttu-id="aa29a-104">Criar um objeto countriesRegions no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="aa29a-104">Create a countriesRegions object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa29a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="aa29a-105">Permissions</span></span>
<span data-ttu-id="aa29a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa29a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa29a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa29a-108">Permission type</span></span> |<span data-ttu-id="aa29a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="aa29a-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="aa29a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa29a-110">Delegated (work or school account)</span></span>|<span data-ttu-id="aa29a-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa29a-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="aa29a-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="aa29a-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="aa29a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa29a-113">Not supported.</span></span>|
|<span data-ttu-id="aa29a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa29a-114">Application</span></span>|<span data-ttu-id="aa29a-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa29a-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa29a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa29a-116">HTTP request</span></span>
```
POST /financials/companies('{id}')/countriesRegions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aa29a-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aa29a-117">Optional query parameters</span></span>
<span data-ttu-id="aa29a-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aa29a-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aa29a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa29a-119">Request headers</span></span>
|<span data-ttu-id="aa29a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa29a-120">Header</span></span>|<span data-ttu-id="aa29a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="aa29a-121">Value</span></span>|
|------|-----|
|<span data-ttu-id="aa29a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa29a-122">Authorization</span></span>  |<span data-ttu-id="aa29a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa29a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="aa29a-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aa29a-125">Content-Type</span></span>  |<span data-ttu-id="aa29a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aa29a-126">application/json</span></span>   |

## <a name="request-body"></a><span data-ttu-id="aa29a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa29a-127">Request body</span></span>
<span data-ttu-id="aa29a-128">No corpo da solicitação, forneça uma representação JSON do objeto **countriesRegions** .</span><span class="sxs-lookup"><span data-stu-id="aa29a-128">In the request body, supply a JSON representation of **countriesRegions** object.</span></span>

## <a name="response"></a><span data-ttu-id="aa29a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa29a-129">Response</span></span>
<span data-ttu-id="aa29a-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **countriesRegions** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa29a-130">If successful, this method returns ```201 Created``` response code and a **countriesRegions** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa29a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa29a-131">Example</span></span>

<span data-ttu-id="aa29a-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="aa29a-132">**Request**</span></span>

<span data-ttu-id="aa29a-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa29a-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/countriesRegions
Content-type: application/json

{
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code"
}
```

<span data-ttu-id="aa29a-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="aa29a-134">**Response**</span></span>

<span data-ttu-id="aa29a-135">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa29a-135">Here is an example of the response.</span></span> 

> <span data-ttu-id="aa29a-136">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa29a-136">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aa29a-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa29a-137">All the properties will be returned from an actual call.</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "US",
  "displayName": "USA",
  "addressFormat": "City+County+Post Code",
  "lastModifiedDateTime": "2017-03-14T15:22:31.753Z"
}

```

