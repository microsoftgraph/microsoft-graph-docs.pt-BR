---
title: Criar customerPaymentJournals
description: Cria um objeto de diário de pagamentos do cliente no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: a633ef91fe15b4999285d7290ca6eed8c10846a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454206"
---
# <a name="create-customerpaymentjournals"></a><span data-ttu-id="2ca40-103">Criar customerPaymentJournals</span><span class="sxs-lookup"><span data-stu-id="2ca40-103">Create customerPaymentJournals</span></span>
<span data-ttu-id="2ca40-104">Cria um objeto de diário de pagamento do cliente no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2ca40-104">Creates a customer payment journal object in Dynamics 365 Business Central.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ca40-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ca40-105">Permissions</span></span>
<span data-ttu-id="2ca40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ca40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ca40-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ca40-108">Permission type</span></span> |<span data-ttu-id="2ca40-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ca40-109">Permissions (from least to most privileged)</span></span>|
|:---------------|:------------------------------------------|
|<span data-ttu-id="2ca40-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ca40-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2ca40-111">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca40-111">Financials.ReadWrite.All</span></span> |
|<span data-ttu-id="2ca40-112">Delegado (conta pessoal da Microsoft</span><span class="sxs-lookup"><span data-stu-id="2ca40-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="2ca40-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ca40-113">Not supported.</span></span>|
|<span data-ttu-id="2ca40-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ca40-114">Application</span></span>|<span data-ttu-id="2ca40-115">Financials.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ca40-115">Financials.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ca40-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ca40-116">HTTP request</span></span>

```
POST /financials/companies('{id}')/customerPaymentJournals('{id}')
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ca40-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ca40-117">Optional query parameters</span></span>
<span data-ttu-id="2ca40-118">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca40-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ca40-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca40-119">Request headers</span></span>
|<span data-ttu-id="2ca40-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2ca40-120">Header</span></span>        |<span data-ttu-id="2ca40-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2ca40-121">Value</span></span>                    |
|--------------|-------------------------|
|<span data-ttu-id="2ca40-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ca40-122">Authorization</span></span> |<span data-ttu-id="2ca40-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ca40-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2ca40-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ca40-125">Content-Type</span></span>  |<span data-ttu-id="2ca40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ca40-126">application/json</span></span>         |

## <a name="request-body"></a><span data-ttu-id="2ca40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ca40-127">Request body</span></span>
<span data-ttu-id="2ca40-128">No corpo da solicitação, forneça uma representação JSON do objeto **customerPaymentJournals** .</span><span class="sxs-lookup"><span data-stu-id="2ca40-128">In the request body, supply a JSON representation of **customerPaymentJournals** object.</span></span>

## <a name="response"></a><span data-ttu-id="2ca40-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ca40-129">Response</span></span>
<span data-ttu-id="2ca40-130">Se bem-sucedido, este método retorna ```201 Created``` um código de resposta e um objeto **customerPaymentJournals** no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ca40-130">If successful, this method returns ```201 Created``` response code and a **customerPaymentJournals** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ca40-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2ca40-131">Example</span></span>

<span data-ttu-id="2ca40-132">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="2ca40-132">**Request**</span></span>

<span data-ttu-id="2ca40-133">Veja a seguir um exemplo de uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ca40-133">Here is an example of a request.</span></span>

```json
POST https://graph.microsoft.com/beta/financials/companies('{id}')/customerPaymentJournals
Content-type: application/json

```json
{
  "code": "DEFAULT"
}
```

<span data-ttu-id="2ca40-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="2ca40-134">**Response**</span></span>

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "code": "DEFAULT",
  "displayName": "Default Journal Batch",
  "lastModifiedDateTime": "2017-05-17T11:30:01.313Z"
}
```


