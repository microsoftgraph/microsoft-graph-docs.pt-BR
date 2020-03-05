---
title: Obter fornecedores
description: Obtém um objeto fornecedor no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: apiPageType
ms.openlocfilehash: 87c79a1b91044c23b771ca613e7b93ba79a1fed0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427911"
---
# <a name="get-vendors"></a><span data-ttu-id="75e1d-103">Obter fornecedores</span><span class="sxs-lookup"><span data-stu-id="75e1d-103">Get vendors</span></span>

<span data-ttu-id="75e1d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="75e1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75e1d-105">Recupere as propriedades e os relacionamentos de um objeto fornecedor para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="75e1d-105">Retrieve the properties and relationships of a vendor object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="75e1d-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="75e1d-106">Permissions</span></span>
<span data-ttu-id="75e1d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75e1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75e1d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75e1d-109">Permission type</span></span> |<span data-ttu-id="75e1d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="75e1d-110">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="75e1d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75e1d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="75e1d-112">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75e1d-112">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="75e1d-113">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="75e1d-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="75e1d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75e1d-114">Not supported.</span></span>|
|<span data-ttu-id="75e1d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75e1d-115">Application</span></span>|<span data-ttu-id="75e1d-116">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75e1d-116">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75e1d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75e1d-117">HTTP request</span></span>

```
GET /financials/companies/{id}/vendors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75e1d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="75e1d-118">Optional query parameters</span></span>
<span data-ttu-id="75e1d-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="75e1d-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75e1d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75e1d-120">Request headers</span></span>
|<span data-ttu-id="75e1d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75e1d-121">Header</span></span>|<span data-ttu-id="75e1d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75e1d-122">Value</span></span>|
|------|-----|
|<span data-ttu-id="75e1d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75e1d-123">Authorization</span></span>  |<span data-ttu-id="75e1d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75e1d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="75e1d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75e1d-126">Request body</span></span>
<span data-ttu-id="75e1d-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75e1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75e1d-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="75e1d-128">Response</span></span>
<span data-ttu-id="75e1d-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto **fornecedores** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75e1d-129">If successful, this method returns a `200 OK` response code and a **vendors** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75e1d-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75e1d-130">Example</span></span>

<span data-ttu-id="75e1d-131">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="75e1d-131">**Request**</span></span>

<span data-ttu-id="75e1d-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75e1d-132">Here is an example of the request.</span></span>
```json
GET https://graph.microsoft.com/beta/financials/companies/{id}/vendors/{id}
```

<span data-ttu-id="75e1d-133">**Response**</span><span class="sxs-lookup"><span data-stu-id="75e1d-133">**Response**</span></span>

<span data-ttu-id="75e1d-134">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75e1d-134">Here is an example of the response.</span></span> 

> <span data-ttu-id="75e1d-135">**Observação**: o objeto de resposta mostrado aqui pode ser encurtado com fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="75e1d-135">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75e1d-136">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75e1d-136">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "number": "40000",
  "displayName": "Wide World Importers",
  "address": {
    "street": "51 Radcroft Road",
    "city": "Atlanta",
    "state": "GA",
    "countryLetterCode": "US",
    "postalCode": "31772"
  },
  "phoneNumber": "",
  "email": "toby.rhode@cronuscorp.net",
  "website": "",
  "taxRegistrationNumber": "",
  "currencyId": "id-value",
  "currencyCode": "USD",
  "irs1099Code": "",
  "paymentTermsId": "id-value",
  "paymentMethodId": "id-value",
  "taxLiable": true,
  "blocked": " ",
  "balance": 0,
  "lastModifiedDateTime": "2017-03-07T00:35:29.667Z"
}
```


