---
title: Tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas PSTN (Rede Telefônica pública de Comutr).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 584efcd6e320a95dc6e62f59b112d1041535f054
ms.sourcegitcommit: fdd69d362d1debc7b08e78269d59b531f9dfdaae
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697169"
---
# <a name="pstncalllogrow-resource-type"></a><span data-ttu-id="03213-103">Tipo de recurso pstnCallLogRow</span><span class="sxs-lookup"><span data-stu-id="03213-103">pstnCallLogRow resource type</span></span>

<span data-ttu-id="03213-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="03213-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03213-105">Representa uma linha de dados no log de chamadas PSTN (Rede Telefônica pública de Comutr).</span><span class="sxs-lookup"><span data-stu-id="03213-105">Represents a row of data in the Public Switch Telephone Network (PSTN) call log.</span></span> <span data-ttu-id="03213-106">Cada linha mapeia para uma chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="03213-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03213-107">Properties</span></span>

|<span data-ttu-id="03213-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03213-108">Property</span></span>|<span data-ttu-id="03213-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="03213-109">Type</span></span>|<span data-ttu-id="03213-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03213-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03213-111">callDurationSource</span><span class="sxs-lookup"><span data-stu-id="03213-111">callDurationSource</span></span>|<span data-ttu-id="03213-112">pstnCallDurationSource</span><span class="sxs-lookup"><span data-stu-id="03213-112">pstnCallDurationSource</span></span>|<span data-ttu-id="03213-113">A origem dos dados de duração da chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-113">The source of the call duration data.</span></span> <span data-ttu-id="03213-114">Se a chamada usar um operador de telecomunicações de terceiros por meio do Programa de Conexão do Operador, o operador poderá fornecer seus próprios dados de duração da chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-114">If the call uses a third-party telecommunications operator via the Operator Connect Program, the operator may provide their own call duration data.</span></span> <span data-ttu-id="03213-115">Nesse caso, o valor da propriedade é `operator` .</span><span class="sxs-lookup"><span data-stu-id="03213-115">In this case, the property value is `operator`.</span></span> <span data-ttu-id="03213-116">Caso contrário, o valor será `microsoft` .</span><span class="sxs-lookup"><span data-stu-id="03213-116">Otherwise, the value is `microsoft`.</span></span>|
|<span data-ttu-id="03213-117">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="03213-117">calleeNumber</span></span>|<span data-ttu-id="03213-118">String</span><span class="sxs-lookup"><span data-stu-id="03213-118">String</span></span>|<span data-ttu-id="03213-119">Número discado no [formato E.164.](https://en.wikipedia.org/wiki/E.164)</span><span class="sxs-lookup"><span data-stu-id="03213-119">Number dialed in [E.164](https://en.wikipedia.org/wiki/E.164) format.</span></span>|
|<span data-ttu-id="03213-120">callerNumber</span><span class="sxs-lookup"><span data-stu-id="03213-120">callerNumber</span></span>|<span data-ttu-id="03213-121">String</span><span class="sxs-lookup"><span data-stu-id="03213-121">String</span></span>|<span data-ttu-id="03213-122">Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída.</span><span class="sxs-lookup"><span data-stu-id="03213-122">Number that received the call for inbound calls or the number dialed for outbound calls.</span></span> <span data-ttu-id="03213-123">Formato E.164.</span><span class="sxs-lookup"><span data-stu-id="03213-123">E.164 format.</span></span>|
|<span data-ttu-id="03213-124">callId</span><span class="sxs-lookup"><span data-stu-id="03213-124">callId</span></span>|<span data-ttu-id="03213-125">String</span><span class="sxs-lookup"><span data-stu-id="03213-125">String</span></span>|<span data-ttu-id="03213-126">Identificador de chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-126">Call identifier.</span></span> <span data-ttu-id="03213-127">Não é garantido que seja exclusivo.</span><span class="sxs-lookup"><span data-stu-id="03213-127">Not guaranteed to be unique.</span></span>|
|<span data-ttu-id="03213-128">callType</span><span class="sxs-lookup"><span data-stu-id="03213-128">callType</span></span>|<span data-ttu-id="03213-129">String</span><span class="sxs-lookup"><span data-stu-id="03213-129">String</span></span>|<span data-ttu-id="03213-130">Se a chamada foi uma chamada de saída ou de entrada PSTN e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="03213-130">Whether the call was a PSTN outbound or inbound call and the type of call such as a call placed by a user or an audio conference.</span></span>|
|<span data-ttu-id="03213-131">charge</span><span class="sxs-lookup"><span data-stu-id="03213-131">charge</span></span>|<span data-ttu-id="03213-132">Duplo</span><span class="sxs-lookup"><span data-stu-id="03213-132">Double</span></span>|<span data-ttu-id="03213-133">Quantidade de dinheiro ou custo da chamada que é cobrada em sua conta.</span><span class="sxs-lookup"><span data-stu-id="03213-133">Amount of money or cost of the call that is charged to your account.</span></span>|
|<span data-ttu-id="03213-134">conferenceId</span><span class="sxs-lookup"><span data-stu-id="03213-134">conferenceId</span></span>|<span data-ttu-id="03213-135">String</span><span class="sxs-lookup"><span data-stu-id="03213-135">String</span></span>|<span data-ttu-id="03213-136">ID da conferência de áudio.</span><span class="sxs-lookup"><span data-stu-id="03213-136">ID of the audio conference.</span></span>|
|<span data-ttu-id="03213-137">connectionCharge</span><span class="sxs-lookup"><span data-stu-id="03213-137">connectionCharge</span></span>|<span data-ttu-id="03213-138">Duplo</span><span class="sxs-lookup"><span data-stu-id="03213-138">Double</span></span>|<span data-ttu-id="03213-139">Preço da taxa de conexão.</span><span class="sxs-lookup"><span data-stu-id="03213-139">Connection fee price.</span></span>|
|<span data-ttu-id="03213-140">currency</span><span class="sxs-lookup"><span data-stu-id="03213-140">currency</span></span>|<span data-ttu-id="03213-141">String</span><span class="sxs-lookup"><span data-stu-id="03213-141">String</span></span>|<span data-ttu-id="03213-142">Tipo de moeda usada para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span><span class="sxs-lookup"><span data-stu-id="03213-142">Type of currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).</span></span>|
|<span data-ttu-id="03213-143">destinationContext</span><span class="sxs-lookup"><span data-stu-id="03213-143">destinationContext</span></span>|<span data-ttu-id="03213-144">String</span><span class="sxs-lookup"><span data-stu-id="03213-144">String</span></span>|<span data-ttu-id="03213-145">Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base na localização do usuário.</span><span class="sxs-lookup"><span data-stu-id="03213-145">Whether the call was domestic (within a country or region) or international (outside a country or region) based on the user's location.</span></span>|
|<span data-ttu-id="03213-146">destinationName</span><span class="sxs-lookup"><span data-stu-id="03213-146">destinationName</span></span>|<span data-ttu-id="03213-147">String</span><span class="sxs-lookup"><span data-stu-id="03213-147">String</span></span>|<span data-ttu-id="03213-148">País ou região discada.</span><span class="sxs-lookup"><span data-stu-id="03213-148">Country or region dialed.</span></span>|
|<span data-ttu-id="03213-149">duração</span><span class="sxs-lookup"><span data-stu-id="03213-149">duration</span></span>|<span data-ttu-id="03213-150">Int32</span><span class="sxs-lookup"><span data-stu-id="03213-150">Int32</span></span>|<span data-ttu-id="03213-151">Por quanto tempo a chamada foi conectada, em segundos.</span><span class="sxs-lookup"><span data-stu-id="03213-151">How long the call was connected, in seconds.</span></span>|
|<span data-ttu-id="03213-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="03213-152">endDateTime</span></span>|<span data-ttu-id="03213-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03213-153">DateTimeOffset</span></span>|<span data-ttu-id="03213-154">Hora da finalização da chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-154">Call end time.</span></span>|
|<span data-ttu-id="03213-155">id</span><span class="sxs-lookup"><span data-stu-id="03213-155">id</span></span>|<span data-ttu-id="03213-156">String</span><span class="sxs-lookup"><span data-stu-id="03213-156">String</span></span>|<span data-ttu-id="03213-157">Identificador de chamada exclusivo.</span><span class="sxs-lookup"><span data-stu-id="03213-157">Unique call identifier.</span></span> <span data-ttu-id="03213-158">GUID.</span><span class="sxs-lookup"><span data-stu-id="03213-158">GUID.</span></span>|
|<span data-ttu-id="03213-159">inventoryType</span><span class="sxs-lookup"><span data-stu-id="03213-159">inventoryType</span></span>|<span data-ttu-id="03213-160">String</span><span class="sxs-lookup"><span data-stu-id="03213-160">String</span></span>|<span data-ttu-id="03213-161">Tipo de número de telefone do usuário, como um serviço de número de chamada gratuita.</span><span class="sxs-lookup"><span data-stu-id="03213-161">User's phone number type, such as a service of toll-free number.</span></span>|
|<span data-ttu-id="03213-162">licenseCapability</span><span class="sxs-lookup"><span data-stu-id="03213-162">licenseCapability</span></span>|<span data-ttu-id="03213-163">String</span><span class="sxs-lookup"><span data-stu-id="03213-163">String</span></span>|<span data-ttu-id="03213-164">A licença usada para a chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-164">The license used for the call.</span></span>|
|<span data-ttu-id="03213-165">operator</span><span class="sxs-lookup"><span data-stu-id="03213-165">operator</span></span>|<span data-ttu-id="03213-166">String</span><span class="sxs-lookup"><span data-stu-id="03213-166">String</span></span>|<span data-ttu-id="03213-167">O operador de telecomunicações que forneceu serviços PSTN para essa chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-167">The telecommunications operator which provided PSTN services for this call.</span></span> <span data-ttu-id="03213-168">Pode ser a Microsoft ou pode ser um operador de terceiros por meio do [Programa de Conexão do Operador.](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)</span><span class="sxs-lookup"><span data-stu-id="03213-168">This may be Microsoft, or it may be a third-party operator via the [Operator Connect Program](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398).</span></span>|
|<span data-ttu-id="03213-169">startDateTime</span><span class="sxs-lookup"><span data-stu-id="03213-169">startDateTime</span></span>|<span data-ttu-id="03213-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03213-170">DateTimeOffset</span></span>|<span data-ttu-id="03213-171">Hora do início da chamada.</span><span class="sxs-lookup"><span data-stu-id="03213-171">Call start time.</span></span>|
|<span data-ttu-id="03213-172">tenantCountryCode</span><span class="sxs-lookup"><span data-stu-id="03213-172">tenantCountryCode</span></span>|<span data-ttu-id="03213-173">String</span><span class="sxs-lookup"><span data-stu-id="03213-173">String</span></span>|<span data-ttu-id="03213-174">Código de país do locatário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="03213-174">Country code of the tenant, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="03213-175">usageCountryCode</span><span class="sxs-lookup"><span data-stu-id="03213-175">usageCountryCode</span></span>|<span data-ttu-id="03213-176">String</span><span class="sxs-lookup"><span data-stu-id="03213-176">String</span></span>|<span data-ttu-id="03213-177">Código de país do usuário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span><span class="sxs-lookup"><span data-stu-id="03213-177">Country code of the user, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).</span></span>|
|<span data-ttu-id="03213-178">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="03213-178">userDisplayName</span></span>|<span data-ttu-id="03213-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03213-179">String</span></span>|<span data-ttu-id="03213-180">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="03213-180">Display name of the user.</span></span>|
|<span data-ttu-id="03213-181">userId</span><span class="sxs-lookup"><span data-stu-id="03213-181">userId</span></span>|<span data-ttu-id="03213-182">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03213-182">String</span></span>|<span data-ttu-id="03213-183">Chamando a ID do usuário no Graph.</span><span class="sxs-lookup"><span data-stu-id="03213-183">Calling user's ID in Graph.</span></span> <span data-ttu-id="03213-184">GUID.</span><span class="sxs-lookup"><span data-stu-id="03213-184">GUID.</span></span> <span data-ttu-id="03213-185">Essa e outras informações de usuário serão nulas/vazias para tipos de chamada de bot (ucap_in, ucap_out).</span><span class="sxs-lookup"><span data-stu-id="03213-185">This and other user info will be null/empty for bot call types (ucap_in, ucap_out).</span></span>|
|<span data-ttu-id="03213-186">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03213-186">userPrincipalName</span></span>|<span data-ttu-id="03213-187">String</span><span class="sxs-lookup"><span data-stu-id="03213-187">String</span></span>|<span data-ttu-id="03213-188">UserPrincipalName (nome de login) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03213-188">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="03213-189">Isso geralmente é o mesmo que o Endereço SIP do usuário e pode ser igual ao endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="03213-189">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03213-190">Relações</span><span class="sxs-lookup"><span data-stu-id="03213-190">Relationships</span></span>

<span data-ttu-id="03213-191">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03213-191">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03213-192">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03213-192">JSON representation</span></span>

<span data-ttu-id="03213-193">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03213-193">The following is a JSON representation of the resource.</span></span>

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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


