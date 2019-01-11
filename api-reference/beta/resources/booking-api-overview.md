---
title: Use a API do reservas Microsoft no Microsoft Graph
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845532"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="eaac2-104">Use a API do reservas Microsoft no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="eaac2-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 > <span data-ttu-id="eaac2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaac2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaac2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaac2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="eaac2-107">Microsoft Bookings permite que os proprietários de pequenas empresas gerencie informações com uma configuração mínima e reservas de cliente.</span><span class="sxs-lookup"><span data-stu-id="eaac2-107">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="eaac2-108">Um proprietário de negócios pode criar uma ou mais empresas, com cada empresa que oferece um conjunto de serviços.</span><span class="sxs-lookup"><span data-stu-id="eaac2-108">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="eaac2-109">O proprietário pode configurar membros da equipe e especifique os serviços que cada membro da equipe realiza.</span><span class="sxs-lookup"><span data-stu-id="eaac2-109">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="eaac2-110">Um cliente pode agendar um compromisso para um serviço específico em que os negócios em um aplicativo online ou móvel.</span><span class="sxs-lookup"><span data-stu-id="eaac2-110">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="eaac2-111">Reservas garante que a hora do compromisso é mantida atualizada para os negócios, os membros da equipe e clientes envolvido.</span><span class="sxs-lookup"><span data-stu-id="eaac2-111">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="eaac2-112">Programaticamente, um [bookingBusiness](bookingbusiness.md) na API reservas envolve os seguintes objetos:</span><span class="sxs-lookup"><span data-stu-id="eaac2-112">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="eaac2-113">Um ou mais objetos [bookingStaffMember](bookingstaffmember.md)</span><span class="sxs-lookup"><span data-stu-id="eaac2-113">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="eaac2-114">Um ou mais objetos [bookingService](bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="eaac2-114">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="eaac2-115">Um conjunto de instâncias de [bookingAppointment](bookingappointment.md)</span><span class="sxs-lookup"><span data-stu-id="eaac2-115">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="eaac2-116">Um conjunto de objetos [bookingCustomer](bookingcustomer.md)</span><span class="sxs-lookup"><span data-stu-id="eaac2-116">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="eaac2-117">Usando as API REST reservas</span><span class="sxs-lookup"><span data-stu-id="eaac2-117">Using the Bookings REST API</span></span>

<span data-ttu-id="eaac2-118">Explore as etapas a seguir antes de compromissos do cliente para uma empresa de reserva na primeira vez.</span><span class="sxs-lookup"><span data-stu-id="eaac2-118">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="eaac2-119">Verifique se que você fornecer [tokens de acesso](/graph/auth-overview) apropriado para as operações correspondentes.</span><span class="sxs-lookup"><span data-stu-id="eaac2-119">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="eaac2-120">Verifique se que a empresa tem uma assinatura do [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) .</span><span class="sxs-lookup"><span data-stu-id="eaac2-120">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="eaac2-121">Crie um novo **bookingBusiness** enviando uma operação POST no conjunto de entidade.</span><span class="sxs-lookup"><span data-stu-id="eaac2-121">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="eaac2-122">No mínimo, você deve especificar um nome para o novo negócio que os clientes verão:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="eaac2-122">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="eaac2-123">Use a propriedade **id** do novo **bookingBusiness** retornados na resposta POST para continuar para [Personalizar](../api/bookingbusiness-update.md) configurações de negócios e adicionar membros da equipe e serviços para a empresa.</span><span class="sxs-lookup"><span data-stu-id="eaac2-123">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="eaac2-124">Adicione membros da equipe individuais para os negócios:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="eaac2-124">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
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
4. <span data-ttu-id="eaac2-125">Defina cada serviço oferecido pela empresa:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="eaac2-125">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="eaac2-126">Publica a página de agendamento para os negócios, para permitir que os clientes e iniciar o agendamento de compromissos de operadores de negócios:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="eaac2-126">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="eaac2-127">Em geral, para listar todas as empresas de reserva em inquilino do Office 365:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="eaac2-127">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="eaac2-128">Casos comuns de uso</span><span class="sxs-lookup"><span data-stu-id="eaac2-128">Common use cases</span></span> 

<span data-ttu-id="eaac2-129">A tabela a seguir lista as operações comuns para uma empresa na API reservas.</span><span class="sxs-lookup"><span data-stu-id="eaac2-129">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="eaac2-130">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="eaac2-130">Use cases</span></span>        | <span data-ttu-id="eaac2-131">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="eaac2-131">REST resources</span></span> | <span data-ttu-id="eaac2-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="eaac2-132">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="eaac2-133">Criar, obter, atualizar ou excluir uma empresa</span><span class="sxs-lookup"><span data-stu-id="eaac2-133">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="eaac2-134">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="eaac2-134">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="eaac2-135">Métodos de bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="eaac2-135">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="eaac2-136">Atualizar a política de agendamento</span><span class="sxs-lookup"><span data-stu-id="eaac2-136">Update the scheduling policy</span></span> | [<span data-ttu-id="eaac2-137">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="eaac2-137">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="eaac2-138">Atualizar um bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="eaac2-138">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="eaac2-139">Adicionar, obter, atualizar ou excluir membros da equipe</span><span class="sxs-lookup"><span data-stu-id="eaac2-139">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="eaac2-140">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="eaac2-140">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="eaac2-141">Métodos de bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="eaac2-141">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="eaac2-142">Adicionar, obter, atualizar ou excluir serviços</span><span class="sxs-lookup"><span data-stu-id="eaac2-142">Add, get, update, or delete services</span></span> | [<span data-ttu-id="eaac2-143">bookingService</span><span class="sxs-lookup"><span data-stu-id="eaac2-143">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="eaac2-144">Métodos de bookingService</span><span class="sxs-lookup"><span data-stu-id="eaac2-144">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="eaac2-145">Publicar ou cancelar a publicação de página de agendamento</span><span class="sxs-lookup"><span data-stu-id="eaac2-145">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="eaac2-146">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="eaac2-146">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="eaac2-147">Publicar</span><span class="sxs-lookup"><span data-stu-id="eaac2-147">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="eaac2-148">cancelamento de publicação</span><span class="sxs-lookup"><span data-stu-id="eaac2-148">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="eaac2-149">Criar, obter, atualizar, excluir ou cancelar um compromisso</span><span class="sxs-lookup"><span data-stu-id="eaac2-149">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="eaac2-150">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="eaac2-150">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="eaac2-151">Métodos de bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="eaac2-151">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="eaac2-152">Obter compromissos em um intervalo de datas</span><span class="sxs-lookup"><span data-stu-id="eaac2-152">Get appointments in a date range</span></span> | [<span data-ttu-id="eaac2-153">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="eaac2-153">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="eaac2-154">Lista reservas calendarView</span><span class="sxs-lookup"><span data-stu-id="eaac2-154">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="eaac2-155">Obtenha a moeda</span><span class="sxs-lookup"><span data-stu-id="eaac2-155">Get currency</span></span> | [<span data-ttu-id="eaac2-156">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="eaac2-156">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="eaac2-157">Métodos de bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="eaac2-157">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="eaac2-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="eaac2-158">See also</span></span>

- <span data-ttu-id="eaac2-159">Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="eaac2-159">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="eaac2-160">Consulte [como alguns dos nossos parceiros estão usando o Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span><span class="sxs-lookup"><span data-stu-id="eaac2-160">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="eaac2-161">Saiba como escolher as [permissões](/graph/permissions-reference) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="eaac2-161">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
