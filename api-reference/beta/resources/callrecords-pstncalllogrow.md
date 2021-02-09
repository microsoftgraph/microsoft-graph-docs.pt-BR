---
title: Tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas da PSTN (Rede Telefônica Pública comu pt-br).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155577"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="5ce03-103">Tipo de recurso pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="5ce03-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="5ce03-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="5ce03-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ce03-105">Representa uma linha de dados no log de chamadas da PSTN (Rede Telefônica Pública comu pt-br).</span><span class="sxs-lookup"><span data-stu-id="5ce03-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="5ce03-106">Cada linha mapeia para uma chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="5ce03-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ce03-107">Properties</span></span>

|<span data-ttu-id="5ce03-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ce03-108">Property</span></span>|<span data-ttu-id="5ce03-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ce03-109">Type</span></span>|<span data-ttu-id="5ce03-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ce03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ce03-111">id</span><span class="sxs-lookup"><span data-stu-id="5ce03-111">id</span></span>|<span data-ttu-id="5ce03-112">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-112">String</span></span>|<span data-ttu-id="5ce03-113">Identificador exclusivo da chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-113">Unique call identifier.</span></span> <span data-ttu-id="5ce03-114">GUID.</span><span class="sxs-lookup"><span data-stu-id="5ce03-114">GUID.</span></span>|
|<span data-ttu-id="5ce03-115">callId</span><span class="sxs-lookup"><span data-stu-id="5ce03-115">callId</span></span>|<span data-ttu-id="5ce03-116">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-116">String</span></span>|<span data-ttu-id="5ce03-117">Identificador de chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-117">Call identifier.</span></span> <span data-ttu-id="5ce03-118">Não há garantia de ser exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5ce03-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="5ce03-119">userId</span><span class="sxs-lookup"><span data-stu-id="5ce03-119">userId</span></span>|<span data-ttu-id="5ce03-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ce03-120">String</span></span>|<span data-ttu-id="5ce03-121">Chamar a ID do usuário no Graph.</span><span class="sxs-lookup"><span data-stu-id="5ce03-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="5ce03-122">GUID.</span><span class="sxs-lookup"><span data-stu-id="5ce03-122">GUID.</span></span> <span data-ttu-id="5ce03-123">Essa e outras informações do usuário serão nulas/vazias para tipos de chamada de bot (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="5ce03-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="5ce03-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ce03-124">userPrincipalName</span></span>|<span data-ttu-id="5ce03-125">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-125">String</span></span>|<span data-ttu-id="5ce03-126">UserPrincipalName (nome de login) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5ce03-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="5ce03-127">Isso geralmente é o mesmo endereço SIP do usuário e pode ser igual ao endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ce03-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="5ce03-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ce03-128">userDisplayName</span></span>|<span data-ttu-id="5ce03-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ce03-129">String</span></span>|<span data-ttu-id="5ce03-130">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ce03-130">Display name of the user.</span></span>|
|<span data-ttu-id="5ce03-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5ce03-131">startDateTime</span></span>|<span data-ttu-id="5ce03-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ce03-132">DateTimeOffset</span></span>|<span data-ttu-id="5ce03-133">Hora do início da chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-133">Call start time.</span></span>|
|<span data-ttu-id="5ce03-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="5ce03-134">endDateTime</span></span>|<span data-ttu-id="5ce03-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ce03-135">DateTimeOffset</span></span>|<span data-ttu-id="5ce03-136">Hora da finalização da chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-136">Call end time.</span></span>|
|<span data-ttu-id="5ce03-137">duração</span><span class="sxs-lookup"><span data-stu-id="5ce03-137">duration</span></span>|<span data-ttu-id="5ce03-138">Int32</span><span class="sxs-lookup"><span data-stu-id="5ce03-138">Int32</span></span>|<span data-ttu-id="5ce03-139">Quanto tempo a chamada foi conectada, em segundos.</span><span class="sxs-lookup"><span data-stu-id="5ce03-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="5ce03-140">charge</span><span class="sxs-lookup"><span data-stu-id="5ce03-140">charge</span></span>|<span data-ttu-id="5ce03-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ce03-141">Double</span></span>|<span data-ttu-id="5ce03-142">Valor em dinheiro ou custo da chamada que é cobrada em sua conta.</span><span class="sxs-lookup"><span data-stu-id="5ce03-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="5ce03-143">callType</span><span class="sxs-lookup"><span data-stu-id="5ce03-143">callType</span></span>|<span data-ttu-id="5ce03-144">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-144">String</span></span>|<span data-ttu-id="5ce03-145">Se a chamada foi uma chamada de saída ou de entrada PSTN e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="5ce03-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="5ce03-146">currency</span><span class="sxs-lookup"><span data-stu-id="5ce03-146">currency</span></span>|<span data-ttu-id="5ce03-147">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-147">String</span></span>|<span data-ttu-id="5ce03-148">Tipo de moeda usado para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span><span class="sxs-lookup"><span data-stu-id="5ce03-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="5ce03-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="5ce03-149">calleeNumber</span></span>|<span data-ttu-id="5ce03-150">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-150">String</span></span>|<span data-ttu-id="5ce03-151">Número discado no [formato E.164.](https://en.wikipedia.org/wiki/E.164)</span><span class="sxs-lookup"><span data-stu-id="5ce03-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="5ce03-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="5ce03-152">usageCountryCode</span></span>|<span data-ttu-id="5ce03-153">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-153">String</span></span>|<span data-ttu-id="5ce03-154">Código do país do usuário, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="5ce03-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="5ce03-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="5ce03-155">tenantCountryCode</span></span>|<span data-ttu-id="5ce03-156">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-156">String</span></span>|<span data-ttu-id="5ce03-157">Código do país do locatário, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="5ce03-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="5ce03-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="5ce03-158">connectionCharge</span></span>|<span data-ttu-id="5ce03-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="5ce03-159">Double</span></span>|<span data-ttu-id="5ce03-160">Preço da taxa de conexão.</span><span class="sxs-lookup"><span data-stu-id="5ce03-160">Connection fee price.</span></span>|
|<span data-ttu-id="5ce03-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="5ce03-161">callerNumber</span></span>|<span data-ttu-id="5ce03-162">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-162">String</span></span>|<span data-ttu-id="5ce03-163">Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída.</span><span class="sxs-lookup"><span data-stu-id="5ce03-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="5ce03-164">Formato E.164.</span><span class="sxs-lookup"><span data-stu-id="5ce03-164">E.164 format.</span></span>|
|<span data-ttu-id="5ce03-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="5ce03-165">destinationContext</span></span>|<span data-ttu-id="5ce03-166">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-166">String</span></span>|<span data-ttu-id="5ce03-167">Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base na localização do usuário.</span><span class="sxs-lookup"><span data-stu-id="5ce03-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="5ce03-168">destinationName</span><span class="sxs-lookup"><span data-stu-id="5ce03-168">destinationName</span></span>|<span data-ttu-id="5ce03-169">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-169">String</span></span>|<span data-ttu-id="5ce03-170">País ou região discada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-170">Country or region dialed.</span></span>|
|<span data-ttu-id="5ce03-171">conferenceId</span><span class="sxs-lookup"><span data-stu-id="5ce03-171">conferenceId</span></span>|<span data-ttu-id="5ce03-172">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-172">String</span></span>|<span data-ttu-id="5ce03-173">ID da audioconferência.</span><span class="sxs-lookup"><span data-stu-id="5ce03-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="5ce03-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="5ce03-174">licenseCapability</span></span>|<span data-ttu-id="5ce03-175">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-175">String</span></span>|<span data-ttu-id="5ce03-176">A licença usada para a chamada.</span><span class="sxs-lookup"><span data-stu-id="5ce03-176">The license used for the call.</span></span>|
|<span data-ttu-id="5ce03-177">inventoryType</span><span class="sxs-lookup"><span data-stu-id="5ce03-177">inventoryType</span></span>|<span data-ttu-id="5ce03-178">String</span><span class="sxs-lookup"><span data-stu-id="5ce03-178">String</span></span>|<span data-ttu-id="5ce03-179">Tipo de número de telefone do usuário, como um serviço de número gratuito.</span><span class="sxs-lookup"><span data-stu-id="5ce03-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ce03-180">Relações</span><span class="sxs-lookup"><span data-stu-id="5ce03-180">Relationships</span></span>

<span data-ttu-id="5ce03-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ce03-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ce03-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ce03-182">JSON representation</span></span>

<span data-ttu-id="5ce03-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ce03-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```


