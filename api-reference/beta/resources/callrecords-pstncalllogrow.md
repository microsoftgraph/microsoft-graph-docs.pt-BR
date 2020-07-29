---
title: tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN).
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdcaaa311ea3d1f875bd3933420cfed058ef7808
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509966"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="a3576-103">tipo de recurso pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="a3576-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="a3576-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="a3576-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3576-105">Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN).</span><span class="sxs-lookup"><span data-stu-id="a3576-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="a3576-106">Cada linha é mapeada para uma chamada.</span><span class="sxs-lookup"><span data-stu-id="a3576-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="a3576-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3576-107">Properties</span></span>

|<span data-ttu-id="a3576-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a3576-108">Property</span></span>|<span data-ttu-id="a3576-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3576-109">Type</span></span>|<span data-ttu-id="a3576-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3576-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3576-111">id</span><span class="sxs-lookup"><span data-stu-id="a3576-111">id</span></span>|<span data-ttu-id="a3576-112">String</span><span class="sxs-lookup"><span data-stu-id="a3576-112">String</span></span>|<span data-ttu-id="a3576-113">Identificador de chamada exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a3576-113">Unique call identifier.</span></span> <span data-ttu-id="a3576-114">#C0.</span><span class="sxs-lookup"><span data-stu-id="a3576-114">GUID.</span></span>|
|<span data-ttu-id="a3576-115">callId</span><span class="sxs-lookup"><span data-stu-id="a3576-115">callId</span></span>|<span data-ttu-id="a3576-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-116">String</span></span>|<span data-ttu-id="a3576-117">Identificador de chamada.</span><span class="sxs-lookup"><span data-stu-id="a3576-117">Call identifier.</span></span> <span data-ttu-id="a3576-118">Não é garantido como exclusivo.</span><span class="sxs-lookup"><span data-stu-id="a3576-118">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="a3576-119">userId</span><span class="sxs-lookup"><span data-stu-id="a3576-119">userId</span></span>|<span data-ttu-id="a3576-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-120">String</span></span>|<span data-ttu-id="a3576-121">Chamar a ID do usuário no Graph.</span><span class="sxs-lookup"><span data-stu-id="a3576-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="a3576-122">#C0.</span><span class="sxs-lookup"><span data-stu-id="a3576-122">GUID.</span></span> <span data-ttu-id="a3576-123">Esta e outras informações do usuário serão nulas/vazias para tipos de chamada de bot (ucap_in ucap_out).</span><span class="sxs-lookup"><span data-stu-id="a3576-123">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="a3576-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3576-124">userPrincipalName</span></span>|<span data-ttu-id="a3576-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-125">String</span></span>|<span data-ttu-id="a3576-126">UserPrincipalName (nome de entrada) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a3576-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="a3576-127">Isso geralmente é o mesmo que o endereço SIP do usuário e pode ser o mesmo que o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3576-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="a3576-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a3576-128">userDisplayName</span></span>|<span data-ttu-id="a3576-129">String</span><span class="sxs-lookup"><span data-stu-id="a3576-129">String</span></span>|<span data-ttu-id="a3576-130">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3576-130">Display name of the user.</span></span>|
|<span data-ttu-id="a3576-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a3576-131">startDateTime</span></span>|<span data-ttu-id="a3576-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3576-132">DateTimeOffset</span></span>|<span data-ttu-id="a3576-133">Hora do início da chamada.</span><span class="sxs-lookup"><span data-stu-id="a3576-133">Call start time.</span></span>|
|<span data-ttu-id="a3576-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="a3576-134">endDateTime</span></span>|<span data-ttu-id="a3576-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3576-135">DateTimeOffset</span></span>|<span data-ttu-id="a3576-136">Hora da finalização da chamada.</span><span class="sxs-lookup"><span data-stu-id="a3576-136">Call end time.</span></span>|
|<span data-ttu-id="a3576-137">duration</span><span class="sxs-lookup"><span data-stu-id="a3576-137">duration</span></span>|<span data-ttu-id="a3576-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a3576-138">Int32</span></span>|<span data-ttu-id="a3576-139">Quanto tempo a chamada foi conectada, em segundos.</span><span class="sxs-lookup"><span data-stu-id="a3576-139">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="a3576-140">adicional</span><span class="sxs-lookup"><span data-stu-id="a3576-140">charge</span></span>|<span data-ttu-id="a3576-141">Duplo</span><span class="sxs-lookup"><span data-stu-id="a3576-141">Double</span></span>|<span data-ttu-id="a3576-142">Quantidade de dinheiro ou custo da chamada cobrada em sua conta.</span><span class="sxs-lookup"><span data-stu-id="a3576-142">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="a3576-143">callType</span><span class="sxs-lookup"><span data-stu-id="a3576-143">callType</span></span>|<span data-ttu-id="a3576-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-144">String</span></span>|<span data-ttu-id="a3576-145">Se a chamada foi uma chamada PSTN de saída ou de entrada e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a3576-145">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="a3576-146">moeda</span><span class="sxs-lookup"><span data-stu-id="a3576-146">currency</span></span>|<span data-ttu-id="a3576-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-147">String</span></span>|<span data-ttu-id="a3576-148">Tipo de moeda usada para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span><span class="sxs-lookup"><span data-stu-id="a3576-148">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="a3576-149">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="a3576-149">calleeNumber</span></span>|<span data-ttu-id="a3576-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-150">String</span></span>|<span data-ttu-id="a3576-151">Número discado no formato [E. 164](https://en.wikipedia.org/wiki/E.164) .</span><span class="sxs-lookup"><span data-stu-id="a3576-151">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="a3576-152">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="a3576-152">usageCountryCode</span></span>|<span data-ttu-id="a3576-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-153">String</span></span>|<span data-ttu-id="a3576-154">Código do país do usuário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="a3576-154">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="a3576-155">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="a3576-155">tenantCountryCode</span></span>|<span data-ttu-id="a3576-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-156">String</span></span>|<span data-ttu-id="a3576-157">Código do país do locatário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="a3576-157">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="a3576-158">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="a3576-158">connectionCharge</span></span>|<span data-ttu-id="a3576-159">Duplo</span><span class="sxs-lookup"><span data-stu-id="a3576-159">Double</span></span>|<span data-ttu-id="a3576-160">Preço da taxa de conexão.</span><span class="sxs-lookup"><span data-stu-id="a3576-160">Connection fee price.</span></span>|
|<span data-ttu-id="a3576-161">callerNumber</span><span class="sxs-lookup"><span data-stu-id="a3576-161">callerNumber</span></span>|<span data-ttu-id="a3576-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-162">String</span></span>|<span data-ttu-id="a3576-163">Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída.</span><span class="sxs-lookup"><span data-stu-id="a3576-163">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="a3576-164">Formato E. 164.</span><span class="sxs-lookup"><span data-stu-id="a3576-164">E.164 format.</span></span>|
|<span data-ttu-id="a3576-165">destinationContext</span><span class="sxs-lookup"><span data-stu-id="a3576-165">destinationContext</span></span>|<span data-ttu-id="a3576-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-166">String</span></span>|<span data-ttu-id="a3576-167">Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base no local do usuário.</span><span class="sxs-lookup"><span data-stu-id="a3576-167">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="a3576-168">destinationname</span><span class="sxs-lookup"><span data-stu-id="a3576-168">destinationName</span></span>|<span data-ttu-id="a3576-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-169">String</span></span>|<span data-ttu-id="a3576-170">País ou região discada.</span><span class="sxs-lookup"><span data-stu-id="a3576-170">Country or region dialed.</span></span>|
|<span data-ttu-id="a3576-171">ID</span><span class="sxs-lookup"><span data-stu-id="a3576-171">conferenceId</span></span>|<span data-ttu-id="a3576-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-172">String</span></span>|<span data-ttu-id="a3576-173">ID da conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="a3576-173">ID of the audio conference.</span></span>|
|<span data-ttu-id="a3576-174">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="a3576-174">licenseCapability</span></span>|<span data-ttu-id="a3576-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-175">String</span></span>|<span data-ttu-id="a3576-176">A licença usada para a chamada.</span><span class="sxs-lookup"><span data-stu-id="a3576-176">The license used for the call.</span></span>|
|<span data-ttu-id="a3576-177">inventorytype</span><span class="sxs-lookup"><span data-stu-id="a3576-177">inventoryType</span></span>|<span data-ttu-id="a3576-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3576-178">String</span></span>|<span data-ttu-id="a3576-179">Tipo de número de telefone do usuário, como um serviço de número de chamada gratuita.</span><span class="sxs-lookup"><span data-stu-id="a3576-179">User's phone number type, such as a service of toll-free number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3576-180">Relações</span><span class="sxs-lookup"><span data-stu-id="a3576-180">Relationships</span></span>

<span data-ttu-id="a3576-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3576-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3576-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3576-182">JSON representation</span></span>

<span data-ttu-id="a3576-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a3576-183">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
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
