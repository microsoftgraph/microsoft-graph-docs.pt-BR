---
title: Obter bookingCurrency
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 3b39b6ba83f77f9b47661e3bf4a98330b5f7ee0b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855059"
---
# <a name="get-bookingcurrency"></a><span data-ttu-id="7f516-104">Obter bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="7f516-104">Get bookingCurrency</span></span>

 > <span data-ttu-id="7f516-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7f516-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f516-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7f516-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="7f516-107">Obtenha as propriedades de um objeto [bookingCurrency](../resources/bookingcurrency.md) que está disponível para uma empresa Microsoft Bookings.</span><span class="sxs-lookup"><span data-stu-id="7f516-107">Get the properties of a [bookingCurrency](../resources/bookingcurrency.md) object that is available to a Microsoft Bookings business.</span></span> <span data-ttu-id="7f516-108">Use a propriedade **id** , que é o código da moeda, para especificar a moeda.</span><span class="sxs-lookup"><span data-stu-id="7f516-108">Use the **id** property, which is the currency code, to specify the currency.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f516-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="7f516-109">Permissions</span></span>
<span data-ttu-id="7f516-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f516-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f516-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7f516-112">Permission type</span></span>      | <span data-ttu-id="7f516-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7f516-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f516-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7f516-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7f516-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="7f516-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7f516-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7f516-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f516-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f516-117">Not supported.</span></span>   |
|<span data-ttu-id="7f516-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7f516-118">Application</span></span> | <span data-ttu-id="7f516-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7f516-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="7f516-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7f516-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingCurrencies/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f516-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7f516-121">Optional query parameters</span></span>
<span data-ttu-id="7f516-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7f516-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f516-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f516-123">Request headers</span></span>
| <span data-ttu-id="7f516-124">Nome</span><span class="sxs-lookup"><span data-stu-id="7f516-124">Name</span></span>      |<span data-ttu-id="7f516-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f516-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f516-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="7f516-126">Authorization</span></span>  | <span data-ttu-id="7f516-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="7f516-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f516-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7f516-128">Request body</span></span>
<span data-ttu-id="7f516-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7f516-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7f516-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f516-130">Response</span></span>
<span data-ttu-id="7f516-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [bookingCurrency](../resources/bookingcurrency.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7f516-131">If successful, this method returns a `200 OK` response code and [bookingCurrency](../resources/bookingcurrency.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f516-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7f516-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f516-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7f516-133">Request</span></span>
<span data-ttu-id="7f516-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="7f516-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}-->
```http
GET https://graph.microsoft.com/beta/bookingCurrencies/USD
```
##### <a name="response"></a><span data-ttu-id="7f516-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="7f516-135">Response</span></span>
<span data-ttu-id="7f516-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7f516-136">The following is an example of the response.</span></span> <span data-ttu-id="7f516-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="7f516-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7f516-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7f516-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCurrency"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 50

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingCurrencies/$entity",
    "id": "USD",
    "symbol": "$"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingCurrency",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
