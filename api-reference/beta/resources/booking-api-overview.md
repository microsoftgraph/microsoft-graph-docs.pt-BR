---
title: Usar a API do Microsoft Bookings no Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: 171f75d35812176202263659185bd4dca94e06de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974196"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="59c63-104">Usar a API do Microsoft Bookings no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="59c63-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="59c63-105">O Microsoft Bookings permite que proprietários de pequenas empresas gerenciem reservas e informações de clientes com configuração mínima.</span><span class="sxs-lookup"><span data-stu-id="59c63-105">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="59c63-106">Um proprietário de empresa pode criar um ou mais negócios e cada empresa oferece um conjunto de serviços.</span><span class="sxs-lookup"><span data-stu-id="59c63-106">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="59c63-107">O proprietário pode definir membros da equipe e especificar os serviços que cada membro da equipe executará.</span><span class="sxs-lookup"><span data-stu-id="59c63-107">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="59c63-108">Um cliente pode agendar um horário para um serviço específico nesse negócio em um aplicativo online ou móvel.</span><span class="sxs-lookup"><span data-stu-id="59c63-108">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="59c63-109">O Bookings garante que o horário do compromisso seja mantido atualizado para a empresa, funcionários e clientes envolvidos.</span><span class="sxs-lookup"><span data-stu-id="59c63-109">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="59c63-110">Programaticamente, um [bookingBusiness](bookingbusiness.md) na API do Bookings envolve os seguintes objetos:</span><span class="sxs-lookup"><span data-stu-id="59c63-110">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="59c63-111">Uma ou mais objetos [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="59c63-111">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="59c63-112">Uma ou mais objetos [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="59c63-112">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="59c63-113">Um conjunto de instâncias [bookingAppointment](bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="59c63-113">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="59c63-114">Um conjunto de objetos [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="59c63-114">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="59c63-115">Como usar a API REST do Bookings</span><span class="sxs-lookup"><span data-stu-id="59c63-115">Using the Bookings REST API</span></span>

<span data-ttu-id="59c63-116">Siga as etapas a seguir antes de agendar os compromissos do cliente para uma empresa pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="59c63-116">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="59c63-117">Certifique-se de fornecer os [tokens de acesso](/graph/auth-overview) apropriados para as operações correspondentes.</span><span class="sxs-lookup"><span data-stu-id="59c63-117">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="59c63-118">Garanta que a empresa tenha um assinatura do [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium).</span><span class="sxs-lookup"><span data-stu-id="59c63-118">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="59c63-119">Crie um novo **bookingBusiness** enviando uma operação POST para o conjunto de entidades.</span><span class="sxs-lookup"><span data-stu-id="59c63-119">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="59c63-120">No mínimo, você deve especificar um nome para a nova empresa que os clientes verão:</span><span class="sxs-lookup"><span data-stu-id="59c63-120">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="59c63-121">Use a propriedade **id** do novo **bookingBusiness** retornado na resposta do POST para continuar a [personalizar](../api/bookingbusiness-update.md) configurações de negócios e adicionar funcionários e serviços para a empresa.</span><span class="sxs-lookup"><span data-stu-id="59c63-121">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="59c63-122">Adicione membros individuais da equipe para a empresa:</span><span class="sxs-lookup"><span data-stu-id="59c63-122">Add individual staff members for the business:</span></span>
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
4. <span data-ttu-id="59c63-123">Defina cada serviço oferecido pela empresa:</span><span class="sxs-lookup"><span data-stu-id="59c63-123">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="59c63-124">Publique a página de agendamento para a empresa, para permitir que clientes e operadores de negócios comecem a agendar compromissos:</span><span class="sxs-lookup"><span data-stu-id="59c63-124">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="59c63-125">Em geral, para listar todas as empresas de agendamento no locatário do Office 365:</span><span class="sxs-lookup"><span data-stu-id="59c63-125">In general, to list all the booking businesses in the Office 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="59c63-126">Casos de usos comuns</span><span class="sxs-lookup"><span data-stu-id="59c63-126">Common use cases</span></span> 

<span data-ttu-id="59c63-127">A tabela a seguir lista as operações comuns para uma empresa na API do Bookings.</span><span class="sxs-lookup"><span data-stu-id="59c63-127">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="59c63-128">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="59c63-128">Use cases</span></span>        | <span data-ttu-id="59c63-129">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="59c63-129">REST resources</span></span> | <span data-ttu-id="59c63-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="59c63-130">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="59c63-131">Criar, acessar, atualizar ou excluir uma empresa</span><span class="sxs-lookup"><span data-stu-id="59c63-131">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="59c63-132">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59c63-132">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="59c63-133">Métodos de bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59c63-133">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="59c63-134">Atualizar a política de agendamento</span><span class="sxs-lookup"><span data-stu-id="59c63-134">Update the scheduling policy</span></span> | [<span data-ttu-id="59c63-135">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="59c63-135">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="59c63-136">Atualizar um bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59c63-136">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="59c63-137">Adicionar, obter, atualizar ou excluir membros da equipe</span><span class="sxs-lookup"><span data-stu-id="59c63-137">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="59c63-138">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="59c63-138">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="59c63-139">Métodos de bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="59c63-139">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="59c63-140">Adicionar, obter, atualizar ou excluir serviços</span><span class="sxs-lookup"><span data-stu-id="59c63-140">Add, get, update, or delete services</span></span> | [<span data-ttu-id="59c63-141">bookingService</span><span class="sxs-lookup"><span data-stu-id="59c63-141">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="59c63-142">Métodos de bookingService</span><span class="sxs-lookup"><span data-stu-id="59c63-142">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="59c63-143">Publicar ou cancelar a publicação da página de agendamento</span><span class="sxs-lookup"><span data-stu-id="59c63-143">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="59c63-144">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59c63-144">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="59c63-145">publish</span><span class="sxs-lookup"><span data-stu-id="59c63-145">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="59c63-146">unpublish</span><span class="sxs-lookup"><span data-stu-id="59c63-146">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="59c63-147">Criar, obter, atualizar, excluir ou cancelar um compromisso</span><span class="sxs-lookup"><span data-stu-id="59c63-147">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="59c63-148">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="59c63-148">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="59c63-149">Métodos de bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="59c63-149">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="59c63-150">Obter compromissos em um intervalo de datas</span><span class="sxs-lookup"><span data-stu-id="59c63-150">Get appointments in a date range</span></span> | [<span data-ttu-id="59c63-151">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="59c63-151">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="59c63-152">Listar o calendarView do Bookings</span><span class="sxs-lookup"><span data-stu-id="59c63-152">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="59c63-153">Obter moeda</span><span class="sxs-lookup"><span data-stu-id="59c63-153">Get currency</span></span> | [<span data-ttu-id="59c63-154">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="59c63-154">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="59c63-155">Métodos de bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="59c63-155">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="59c63-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="59c63-156">See also</span></span>

- <span data-ttu-id="59c63-157">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="59c63-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="59c63-158">Veja [como alguns de nossos parceiros usam o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="59c63-158">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="59c63-159">Saiba como escolher [permissões](/graph/permissions-reference) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="59c63-159">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
