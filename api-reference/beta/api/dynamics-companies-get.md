---
title: Obter empresas
description: Obtém um objeto Company no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 161c4c3d295437d3a62f1cb2e97c64b3efa99aa6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42431967"
---
# <a name="get-companies"></a><span data-ttu-id="35e29-103">Obter empresas</span><span class="sxs-lookup"><span data-stu-id="35e29-103">Get companies</span></span>

<span data-ttu-id="35e29-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35e29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35e29-105">Recupere as propriedades e os relacionamentos de um objeto de empresas para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="35e29-105">Retrieve the properties and relationships of a companies object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="35e29-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35e29-106">Permissions</span></span>
<span data-ttu-id="35e29-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35e29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35e29-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35e29-109">Permission type</span></span> |<span data-ttu-id="35e29-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35e29-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="35e29-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35e29-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35e29-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35e29-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="35e29-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="35e29-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="35e29-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="35e29-114">Not supported.</span></span>|
|<span data-ttu-id="35e29-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35e29-115">Application</span></span>|<span data-ttu-id="35e29-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35e29-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35e29-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35e29-117">HTTP request</span></span>
```
GET /financials/companies
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35e29-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="35e29-118">Optional query parameters</span></span>
<span data-ttu-id="35e29-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="35e29-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35e29-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35e29-120">Request headers</span></span>
|<span data-ttu-id="35e29-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="35e29-121">Header</span></span>|<span data-ttu-id="35e29-122">Valor</span><span class="sxs-lookup"><span data-stu-id="35e29-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="35e29-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="35e29-123">Authorization</span></span>  |<span data-ttu-id="35e29-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35e29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35e29-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35e29-126">Request body</span></span>
<span data-ttu-id="35e29-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="35e29-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35e29-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="35e29-128">Response</span></span>
<span data-ttu-id="35e29-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de **empresas** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35e29-129">If successful, this method returns a `200 OK` response code and a **companies** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35e29-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35e29-130">Example</span></span>

<span data-ttu-id="35e29-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="35e29-131">**Request**</span></span>

<span data-ttu-id="35e29-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35e29-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies
```

<span data-ttu-id="35e29-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="35e29-133">**Response**</span></span>

<span data-ttu-id="35e29-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35e29-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="35e29-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35e29-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="35e29-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35e29-136">All the properties will be returned from an actual call.</span></span>

```json
{
    "id": "id-value",
    "systemVersion": "17806",
    "name": "CRONUS US",
    "displayName": "CRONUS USA, Inc.",
    "businessProfileId": ""
}
```
