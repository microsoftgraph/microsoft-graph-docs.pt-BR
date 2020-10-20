---
title: tipo de recurso directRoutingLogRow
description: Representa uma linha de dados no log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c5baf5768c7cee9e0525373bb4f7139f6a145acb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601192"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="ee270-103">tipo de recurso directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="ee270-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="ee270-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="ee270-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee270-105">Representa uma linha de dados no log de chamadas de roteamento direto.</span><span class="sxs-lookup"><span data-stu-id="ee270-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="ee270-106">Cada linha é mapeada para uma chamada.</span><span class="sxs-lookup"><span data-stu-id="ee270-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="ee270-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee270-107">Properties</span></span>

|<span data-ttu-id="ee270-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee270-108">Property</span></span>|<span data-ttu-id="ee270-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee270-109">Type</span></span>|<span data-ttu-id="ee270-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee270-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee270-111">id</span><span class="sxs-lookup"><span data-stu-id="ee270-111">id</span></span>|<span data-ttu-id="ee270-112">String</span><span class="sxs-lookup"><span data-stu-id="ee270-112">String</span></span>|<span data-ttu-id="ee270-113">Identificador de chamada exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ee270-113">Unique call identifier.</span></span> <span data-ttu-id="ee270-114">#C0.</span><span class="sxs-lookup"><span data-stu-id="ee270-114">GUID.</span></span>|
|<span data-ttu-id="ee270-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="ee270-115">correlationId</span></span>|<span data-ttu-id="ee270-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee270-116">String</span></span>|<span data-ttu-id="ee270-117">Identificador para a chamada que você pode usar ao chamar o suporte da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ee270-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="ee270-118">#C0.</span><span class="sxs-lookup"><span data-stu-id="ee270-118">GUID.</span></span>|
|<span data-ttu-id="ee270-119">userId</span><span class="sxs-lookup"><span data-stu-id="ee270-119">userId</span></span>|<span data-ttu-id="ee270-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee270-120">String</span></span>|<span data-ttu-id="ee270-121">Chamar a ID do usuário no Graph.</span><span class="sxs-lookup"><span data-stu-id="ee270-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="ee270-122">Esta e outras informações do usuário serão nulas/vazias para tipos de chamada de bot.</span><span class="sxs-lookup"><span data-stu-id="ee270-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="ee270-123">#C0.</span><span class="sxs-lookup"><span data-stu-id="ee270-123">GUID.</span></span>|
|<span data-ttu-id="ee270-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ee270-124">userPrincipalName</span></span>|<span data-ttu-id="ee270-125">String</span><span class="sxs-lookup"><span data-stu-id="ee270-125">String</span></span>|<span data-ttu-id="ee270-126">UserPrincipalName (nome de entrada) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ee270-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="ee270-127">Isso geralmente é o mesmo que o endereço SIP do usuário e pode ser o mesmo que o endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee270-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="ee270-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ee270-128">userDisplayName</span></span>|<span data-ttu-id="ee270-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ee270-129">String</span></span>|<span data-ttu-id="ee270-130">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee270-130">Display name of the user.</span></span>|
|<span data-ttu-id="ee270-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ee270-131">startDateTime</span></span>|<span data-ttu-id="ee270-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee270-132">DateTimeOffset</span></span>|<span data-ttu-id="ee270-133">Hora do início da chamada.</span><span class="sxs-lookup"><span data-stu-id="ee270-133">Call start time.</span></span><br/><span data-ttu-id="ee270-134">Para chamadas com falha e não atendidas, isso pode ser igual ao tempo de convite ou de falha.</span><span class="sxs-lookup"><span data-stu-id="ee270-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="ee270-135">inviteDateTime</span><span class="sxs-lookup"><span data-stu-id="ee270-135">inviteDateTime</span></span>|<span data-ttu-id="ee270-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee270-136">DateTimeOffset</span></span>| <span data-ttu-id="ee270-137">Quando o convite inicial foi enviado.</span><span class="sxs-lookup"><span data-stu-id="ee270-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="ee270-138">failureDateTime</span><span class="sxs-lookup"><span data-stu-id="ee270-138">failureDateTime</span></span>|<span data-ttu-id="ee270-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee270-139">DateTimeOffset</span></span>| <span data-ttu-id="ee270-140">Existe somente para chamadas com falha (não totalmente estabelecidas).</span><span class="sxs-lookup"><span data-stu-id="ee270-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="ee270-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ee270-141">endDateTime</span></span>|<span data-ttu-id="ee270-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee270-142">DateTimeOffset</span></span>| <span data-ttu-id="ee270-143">Existe somente para chamadas bem-sucedidas (totalmente estabelecidas).</span><span class="sxs-lookup"><span data-stu-id="ee270-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="ee270-144">Hora em que a chamada terminou.</span><span class="sxs-lookup"><span data-stu-id="ee270-144">Time when call ended.</span></span>|
|<span data-ttu-id="ee270-145">duração</span><span class="sxs-lookup"><span data-stu-id="ee270-145">duration</span></span>|<span data-ttu-id="ee270-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ee270-146">Int32</span></span>| <span data-ttu-id="ee270-147">Duração da chamada em segundos.</span><span class="sxs-lookup"><span data-stu-id="ee270-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="ee270-148">callType</span><span class="sxs-lookup"><span data-stu-id="ee270-148">callType</span></span>|<span data-ttu-id="ee270-149">String</span><span class="sxs-lookup"><span data-stu-id="ee270-149">String</span></span>| <span data-ttu-id="ee270-150">Tipo de chamada e direção.</span><span class="sxs-lookup"><span data-stu-id="ee270-150">Call type and direction.</span></span>|
|<span data-ttu-id="ee270-151">successfulCall</span><span class="sxs-lookup"><span data-stu-id="ee270-151">successfulCall</span></span>|<span data-ttu-id="ee270-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee270-152">Boolean</span></span>| <span data-ttu-id="ee270-153">Êxito ou tentativa.</span><span class="sxs-lookup"><span data-stu-id="ee270-153">Success or attempt.</span></span>|
|<span data-ttu-id="ee270-154">callerNumber</span><span class="sxs-lookup"><span data-stu-id="ee270-154">callerNumber</span></span>|<span data-ttu-id="ee270-155">String</span><span class="sxs-lookup"><span data-stu-id="ee270-155">String</span></span>| <span data-ttu-id="ee270-156">Número do usuário ou do bot que fez a chamada.</span><span class="sxs-lookup"><span data-stu-id="ee270-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="ee270-157">Formato [e. 164](https://en.wikipedia.org/wiki/E.164) , mas pode incluir dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="ee270-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="ee270-158">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="ee270-158">calleeNumber</span></span>|<span data-ttu-id="ee270-159">String</span><span class="sxs-lookup"><span data-stu-id="ee270-159">String</span></span>| <span data-ttu-id="ee270-160">Número do usuário ou do bot que recebeu a chamada.</span><span class="sxs-lookup"><span data-stu-id="ee270-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="ee270-161">Formato [e. 164](https://en.wikipedia.org/wiki/E.164) , mas pode incluir dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="ee270-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="ee270-162">mediaPathLocation</span><span class="sxs-lookup"><span data-stu-id="ee270-162">mediaPathLocation</span></span>|<span data-ttu-id="ee270-163">String</span><span class="sxs-lookup"><span data-stu-id="ee270-163">String</span></span>| <span data-ttu-id="ee270-164">O datacenter usado para o caminho de mídia em chamada não bypass.</span><span class="sxs-lookup"><span data-stu-id="ee270-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="ee270-165">signalingLocation</span><span class="sxs-lookup"><span data-stu-id="ee270-165">signalingLocation</span></span>|<span data-ttu-id="ee270-166">String</span><span class="sxs-lookup"><span data-stu-id="ee270-166">String</span></span>| <span data-ttu-id="ee270-167">O datacenter usado para sinalização para as chamadas bypass e non-bypass.</span><span class="sxs-lookup"><span data-stu-id="ee270-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="ee270-168">finalSipCode</span><span class="sxs-lookup"><span data-stu-id="ee270-168">finalSipCode</span></span>|<span data-ttu-id="ee270-169">Int32</span><span class="sxs-lookup"><span data-stu-id="ee270-169">Int32</span></span>| <span data-ttu-id="ee270-170">O código com o qual a chamada terminou, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span><span class="sxs-lookup"><span data-stu-id="ee270-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="ee270-171">callEndSubReason</span><span class="sxs-lookup"><span data-stu-id="ee270-171">callEndSubReason</span></span>|<span data-ttu-id="ee270-172">Int32</span><span class="sxs-lookup"><span data-stu-id="ee270-172">Int32</span></span>| <span data-ttu-id="ee270-173">Além dos códigos SIP, a Microsoft possui subcódigos que indicam o problema específico.</span><span class="sxs-lookup"><span data-stu-id="ee270-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="ee270-174">finalSipCodePhrase</span><span class="sxs-lookup"><span data-stu-id="ee270-174">finalSipCodePhrase</span></span>|<span data-ttu-id="ee270-175">String</span><span class="sxs-lookup"><span data-stu-id="ee270-175">String</span></span>| <span data-ttu-id="ee270-176">Descrição do código SIP e do subcódigo da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ee270-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="ee270-177">trunkFullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="ee270-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="ee270-178">String</span><span class="sxs-lookup"><span data-stu-id="ee270-178">String</span></span>| <span data-ttu-id="ee270-179">Nome de domínio totalmente qualificado do controlador de borda da sessão.</span><span class="sxs-lookup"><span data-stu-id="ee270-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="ee270-180">mediaBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="ee270-180">mediaBypassEnabled</span></span>|<span data-ttu-id="ee270-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee270-181">Boolean</span></span>| <span data-ttu-id="ee270-182">Indica se o tronco foi habilitado para bypass de mídia ou não.</span><span class="sxs-lookup"><span data-stu-id="ee270-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee270-183">Relações</span><span class="sxs-lookup"><span data-stu-id="ee270-183">Relationships</span></span>

<span data-ttu-id="ee270-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee270-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee270-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee270-185">JSON representation</span></span>

<span data-ttu-id="ee270-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee270-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```


