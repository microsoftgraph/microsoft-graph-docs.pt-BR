---
title: Obter customerPaymentJournals
description: Obtém um diário de pagamento do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 14d90b40dc7584b50024ff82921242d0213ed790
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458653"
---
# <a name="get-customerpaymentjournals"></a><span data-ttu-id="6e368-103">Obter customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="6e368-103">Get customerPaymentJournals</span></span>
<span data-ttu-id="6e368-104">Recupere as propriedades e os relacionamentos de um objeto de diário de pagamento do cliente para o Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="6e368-104">Retrieve the properties and relationships of a customer payment journal object for Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e368-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="6e368-105">Permissions</span></span>
<span data-ttu-id="6e368-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e368-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e368-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6e368-108">Permission type</span></span> |<span data-ttu-id="6e368-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6e368-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="6e368-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6e368-110">Delegated (work or school account)</span></span>|<span data-ttu-id="6e368-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e368-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="6e368-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6e368-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="6e368-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6e368-113">Not supported.</span></span>|
|<span data-ttu-id="6e368-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6e368-114">Application</span></span>|<span data-ttu-id="6e368-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e368-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e368-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6e368-116">HTTP request</span></span>

```
GET /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6e368-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6e368-117">Optional query parameters</span></span>
<span data-ttu-id="6e368-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6e368-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6e368-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6e368-119">Request headers</span></span>
|<span data-ttu-id="6e368-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6e368-120">Header</span></span>       |<span data-ttu-id="6e368-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6e368-121">Value</span></span>                     |
|-------------|--------------------------|
|<span data-ttu-id="6e368-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6e368-122">Authorization</span></span>|<span data-ttu-id="6e368-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6e368-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6e368-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6e368-125">Request body</span></span>
<span data-ttu-id="6e368-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6e368-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e368-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6e368-127">Response</span></span>
<span data-ttu-id="6e368-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto **customerPaymentJournals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e368-128">If successful, this method returns a `200 OK` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6e368-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6e368-129">Example</span></span>

<span data-ttu-id="6e368-130">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="6e368-130">**Request**</span></span>

<span data-ttu-id="6e368-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6e368-131">Here is an example of the request.</span></span>

```json
GET https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals('{id}')
```

<span data-ttu-id="6e368-132">**Response**</span><span class="sxs-lookup"><span data-stu-id="6e368-132">**Response**</span></span>

<span data-ttu-id="6e368-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6e368-133">Here is an example of the response.</span></span> 

> <span data-ttu-id="6e368-134">**Observação**: o objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6e368-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6e368-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6e368-135">All the properties will be returned from an actual call.</span></span>

```json
{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```
