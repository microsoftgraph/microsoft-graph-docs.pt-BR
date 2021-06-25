---
title: Usar a API do Microsoft Bookings no Microsoft Graph
description: O Microsoft Bookings permite que proprietários de pequenas empresas gerenciem reservas e informações de clientes com configuração mínima.
localization_priority: Priority
author: arvindmicrosoft
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: c21cb95d140fa41711264ec0e6c71b7828b5a709
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118655"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="f9af0-103">Usar a API do Microsoft Bookings no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9af0-103">Use the Microsoft Bookings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="f9af0-104">O Microsoft Bookings permite que proprietários de pequenas empresas gerenciem reservas e informações de clientes com configuração mínima.</span><span class="sxs-lookup"><span data-stu-id="f9af0-104">Microsoft Bookings lets enterprise organization and small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="f9af0-105">Um proprietário de empresa pode criar um ou mais negócios e cada empresa oferece um conjunto de serviços.</span><span class="sxs-lookup"><span data-stu-id="f9af0-105">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="f9af0-106">O proprietário pode definir membros da equipe e especificar os serviços que cada membro da equipe executará.</span><span class="sxs-lookup"><span data-stu-id="f9af0-106">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="f9af0-107">Um cliente pode agendar um horário para um serviço específico nesse negócio em um aplicativo online ou móvel.</span><span class="sxs-lookup"><span data-stu-id="f9af0-107">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="f9af0-108">O Bookings garante que o horário do compromisso seja mantido atualizado para a empresa, funcionários e clientes envolvidos.</span><span class="sxs-lookup"><span data-stu-id="f9af0-108">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="f9af0-109">Programaticamente, um [bookingBusiness](bookingbusiness.md) na API do Bookings envolve os seguintes objetos:</span><span class="sxs-lookup"><span data-stu-id="f9af0-109">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="f9af0-110">Uma ou mais objetos [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="f9af0-110">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="f9af0-111">Uma ou mais objetos [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="f9af0-111">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="f9af0-112">Um conjunto de instâncias [bookingAppointment](bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="f9af0-112">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="f9af0-113">Um conjunto de objetos [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="f9af0-113">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="f9af0-114">Como usar a API REST do Bookings</span><span class="sxs-lookup"><span data-stu-id="f9af0-114">Using the Bookings REST API</span></span>

<span data-ttu-id="f9af0-115">Siga as etapas a seguir antes de agendar os compromissos do cliente para uma empresa pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="f9af0-115">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="f9af0-116">Certifique-se de fornecer os [tokens de acesso](/graph/auth-overview) apropriados para as operações correspondentes.</span><span class="sxs-lookup"><span data-stu-id="f9af0-116">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="f9af0-117">Certifique-se que a empresa tenha um assinatura do [Microsoft 365 Business Premium](https://products.office.com/pt-BR/business/office-365-business-premium).</span><span class="sxs-lookup"><span data-stu-id="f9af0-117">Make sure the business has an [Microsoft 365 Business Premium](https://products.office.com/pt-BR/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="f9af0-118">Crie um novo **bookingBusiness** enviando uma operação POST para o conjunto de entidades.</span><span class="sxs-lookup"><span data-stu-id="f9af0-118">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="f9af0-119">No mínimo, você deve especificar um nome para a nova empresa que os clientes verão:</span><span class="sxs-lookup"><span data-stu-id="f9af0-119">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="f9af0-120">Use a propriedade **id** do novo **bookingBusiness** retornado na resposta do POST para continuar a [personalizar](../api/bookingbusiness-update.md) configurações de negócios e adicionar funcionários e serviços para a empresa.</span><span class="sxs-lookup"><span data-stu-id="f9af0-120">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="f9af0-121">Adicione membros individuais da equipe para a empresa:</span><span class="sxs-lookup"><span data-stu-id="f9af0-121">Add individual staff members for the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="f9af0-122">Defina cada serviço oferecido pela empresa:</span><span class="sxs-lookup"><span data-stu-id="f9af0-122">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="f9af0-123">Publique a página de agendamento para a empresa, para permitir que clientes e operadores de negócios comecem a agendar compromissos:</span><span class="sxs-lookup"><span data-stu-id="f9af0-123">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="f9af0-124">Em geral, para listar todas as empresas de agendamento no locatário do Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="f9af0-124">In general, to list all the booking businesses in the Microsoft 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="f9af0-125">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="f9af0-125">Common use cases</span></span> 

<span data-ttu-id="f9af0-126">A tabela a seguir lista as operações comuns para uma empresa na API do Bookings.</span><span class="sxs-lookup"><span data-stu-id="f9af0-126">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="f9af0-127">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="f9af0-127">Use cases</span></span>        | <span data-ttu-id="f9af0-128">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="f9af0-128">REST resources</span></span> | <span data-ttu-id="f9af0-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9af0-129">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="f9af0-130">Criar, acessar, atualizar ou excluir uma empresa</span><span class="sxs-lookup"><span data-stu-id="f9af0-130">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="f9af0-131">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f9af0-131">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f9af0-132">Métodos de bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f9af0-132">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="f9af0-133">Atualizar a política de agendamento</span><span class="sxs-lookup"><span data-stu-id="f9af0-133">Update the scheduling policy</span></span> | [<span data-ttu-id="f9af0-134">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="f9af0-134">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="f9af0-135">Atualizar um bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f9af0-135">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="f9af0-136">Adicionar, obter, atualizar ou excluir membros da equipe</span><span class="sxs-lookup"><span data-stu-id="f9af0-136">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="f9af0-137">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="f9af0-137">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="f9af0-138">Métodos de bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="f9af0-138">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="f9af0-139">Adicionar, obter, atualizar ou excluir serviços</span><span class="sxs-lookup"><span data-stu-id="f9af0-139">Add, get, update, or delete services</span></span> | [<span data-ttu-id="f9af0-140">bookingService</span><span class="sxs-lookup"><span data-stu-id="f9af0-140">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="f9af0-141">Métodos de bookingService</span><span class="sxs-lookup"><span data-stu-id="f9af0-141">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="f9af0-142">Publicar ou cancelar a publicação da página de agendamento</span><span class="sxs-lookup"><span data-stu-id="f9af0-142">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="f9af0-143">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f9af0-143">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f9af0-144">publish</span><span class="sxs-lookup"><span data-stu-id="f9af0-144">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="f9af0-145">unpublish</span><span class="sxs-lookup"><span data-stu-id="f9af0-145">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="f9af0-146">Criar, obter, atualizar, excluir ou cancelar um compromisso</span><span class="sxs-lookup"><span data-stu-id="f9af0-146">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="f9af0-147">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="f9af0-147">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="f9af0-148">Métodos de bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="f9af0-148">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="f9af0-149">Obter compromissos em um intervalo de datas</span><span class="sxs-lookup"><span data-stu-id="f9af0-149">Get appointments in a date range</span></span> | [<span data-ttu-id="f9af0-150">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f9af0-150">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="f9af0-151">Listar o calendarView do Bookings</span><span class="sxs-lookup"><span data-stu-id="f9af0-151">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="f9af0-152">Obter moeda</span><span class="sxs-lookup"><span data-stu-id="f9af0-152">Get currency</span></span> | [<span data-ttu-id="f9af0-153">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="f9af0-153">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="f9af0-154">Métodos de bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="f9af0-154">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |

## <a name="whats-new"></a><span data-ttu-id="f9af0-155">O que há de novo</span><span class="sxs-lookup"><span data-stu-id="f9af0-155">What's new</span></span>
<span data-ttu-id="f9af0-156">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="f9af0-156">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="f9af0-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9af0-157">See also</span></span>

- <span data-ttu-id="f9af0-158">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="f9af0-158">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="f9af0-159">Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/partners).</span><span class="sxs-lookup"><span data-stu-id="f9af0-159">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/partners).</span></span>
- <span data-ttu-id="f9af0-160">Saiba como escolher [permissões](/graph/permissions-reference) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9af0-160">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>


