---
title: Tipo de recurso directRoutingLogRow
description: Representa uma linha de dados no log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159651"
---
# <a name="directroutinglogrow-resource-type"></a><span data-ttu-id="9aa0f-103">Tipo de recurso directRoutingLogRow</span><span class="sxs-lookup"><span data-stu-id="9aa0f-103">directRoutingLogRow resource type</span></span>

<span data-ttu-id="9aa0f-104">Namespace: microsoft.graph.callRecords</span><span class="sxs-lookup"><span data-stu-id="9aa0f-104">Namespace: microsoft.graph.callRecords</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9aa0f-105">Representa uma linha de dados no log de chamadas de roteamento direto.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-105">Represents a row of data in the direct routing call log.</span></span> <span data-ttu-id="9aa0f-106">Cada linha mapeia para uma chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-106">Each row maps to one call.</span></span>

## <a name="properties"></a><span data-ttu-id="9aa0f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9aa0f-107">Properties</span></span>

|<span data-ttu-id="9aa0f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9aa0f-108">Property</span></span>|<span data-ttu-id="9aa0f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9aa0f-109">Type</span></span>|<span data-ttu-id="9aa0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9aa0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9aa0f-111">id</span><span class="sxs-lookup"><span data-stu-id="9aa0f-111">id</span></span>|<span data-ttu-id="9aa0f-112">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-112">String</span></span>|<span data-ttu-id="9aa0f-113">Identificador exclusivo da chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-113">Unique call identifier.</span></span> <span data-ttu-id="9aa0f-114">GUID.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-114">GUID.</span></span>|
|<span data-ttu-id="9aa0f-115">correlationId</span><span class="sxs-lookup"><span data-stu-id="9aa0f-115">correlationId</span></span>|<span data-ttu-id="9aa0f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa0f-116">String</span></span>|<span data-ttu-id="9aa0f-117">Identificador da chamada que você pode usar ao chamar o Suporte da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-117">Identifier for the call that you can use when calling Microsoft Support.</span></span> <span data-ttu-id="9aa0f-118">GUID.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-118">GUID.</span></span>|
|<span data-ttu-id="9aa0f-119">userId</span><span class="sxs-lookup"><span data-stu-id="9aa0f-119">userId</span></span>|<span data-ttu-id="9aa0f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa0f-120">String</span></span>|<span data-ttu-id="9aa0f-121">Chamar a ID do usuário no Graph.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-121">Calling user's ID in Graph.</span></span> <span data-ttu-id="9aa0f-122">Essa e outras informações do usuário serão nulas/vazias para tipos de chamada de bot.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-122">This and other user info will be null/empty for bot call types.</span></span> <span data-ttu-id="9aa0f-123">GUID.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-123">GUID.</span></span>|
|<span data-ttu-id="9aa0f-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9aa0f-124">userPrincipalName</span></span>|<span data-ttu-id="9aa0f-125">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-125">String</span></span>|<span data-ttu-id="9aa0f-126">UserPrincipalName (nome de login) no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-126">UserPrincipalName (sign-in name) in Azure Active Directory.</span></span> <span data-ttu-id="9aa0f-127">Isso geralmente é o mesmo endereço SIP do usuário e pode ser igual ao endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-127">This is usually the same as user's SIP Address, and can be same as user's e-mail address.</span></span>|
|<span data-ttu-id="9aa0f-128">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="9aa0f-128">userDisplayName</span></span>|<span data-ttu-id="9aa0f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9aa0f-129">String</span></span>|<span data-ttu-id="9aa0f-130">Nome de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-130">Display name of the user.</span></span>|
|<span data-ttu-id="9aa0f-131">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa0f-131">startDateTime</span></span>|<span data-ttu-id="9aa0f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa0f-132">DateTimeOffset</span></span>|<span data-ttu-id="9aa0f-133">Hora do início da chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-133">Call start time.</span></span><br/><span data-ttu-id="9aa0f-134">Para chamadas com falha e não respondidas, isso pode ser igual ao tempo de convite ou falha.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-134">For failed and unanswered calls, this can be equal to invite or failure time.</span></span>|
|<span data-ttu-id="9aa0f-135">inviteDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa0f-135">inviteDateTime</span></span>|<span data-ttu-id="9aa0f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa0f-136">DateTimeOffset</span></span>| <span data-ttu-id="9aa0f-137">Quando o convite inicial foi enviado.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-137">When the initial invite was sent.</span></span>|
|<span data-ttu-id="9aa0f-138">failureDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa0f-138">failureDateTime</span></span>|<span data-ttu-id="9aa0f-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa0f-139">DateTimeOffset</span></span>| <span data-ttu-id="9aa0f-140">Existe apenas para chamadas com falha (não totalmente estabelecidas).</span><span class="sxs-lookup"><span data-stu-id="9aa0f-140">Only exists for failed (not fully established) calls.</span></span>|
|<span data-ttu-id="9aa0f-141">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9aa0f-141">endDateTime</span></span>|<span data-ttu-id="9aa0f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9aa0f-142">DateTimeOffset</span></span>| <span data-ttu-id="9aa0f-143">Existe apenas para chamadas bem-sucedidas (totalmente estabelecidas).</span><span class="sxs-lookup"><span data-stu-id="9aa0f-143">Only exists for successful (fully established) calls.</span></span> <span data-ttu-id="9aa0f-144">Hora em que a chamada terminou.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-144">Time when call ended.</span></span>|
|<span data-ttu-id="9aa0f-145">duração</span><span class="sxs-lookup"><span data-stu-id="9aa0f-145">duration</span></span>|<span data-ttu-id="9aa0f-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9aa0f-146">Int32</span></span>| <span data-ttu-id="9aa0f-147">Duração da chamada em segundos.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-147">Duration of the call in seconds.</span></span>|
|<span data-ttu-id="9aa0f-148">callType</span><span class="sxs-lookup"><span data-stu-id="9aa0f-148">callType</span></span>|<span data-ttu-id="9aa0f-149">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-149">String</span></span>| <span data-ttu-id="9aa0f-150">Tipo e direção da chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-150">Call type and direction.</span></span>|
|<span data-ttu-id="9aa0f-151">successfulCall</span><span class="sxs-lookup"><span data-stu-id="9aa0f-151">successfulCall</span></span>|<span data-ttu-id="9aa0f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aa0f-152">Boolean</span></span>| <span data-ttu-id="9aa0f-153">Sucesso ou tentativa.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-153">Success or attempt.</span></span>|
|<span data-ttu-id="9aa0f-154">callerNumber</span><span class="sxs-lookup"><span data-stu-id="9aa0f-154">callerNumber</span></span>|<span data-ttu-id="9aa0f-155">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-155">String</span></span>| <span data-ttu-id="9aa0f-156">Número do usuário ou bot que fez a chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-156">Number of the user or bot who made the call.</span></span> <span data-ttu-id="9aa0f-157">[Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-157">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="9aa0f-158">calleeNumber</span><span class="sxs-lookup"><span data-stu-id="9aa0f-158">calleeNumber</span></span>|<span data-ttu-id="9aa0f-159">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-159">String</span></span>| <span data-ttu-id="9aa0f-160">Número do usuário ou bot que recebeu a chamada.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-160">Number of the user or bot who received the call.</span></span> <span data-ttu-id="9aa0f-161">[Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-161">[E.164](https://en.wikipedia.org/wiki/E.164) format, but may include additional data.</span></span>|
|<span data-ttu-id="9aa0f-162">mediaPathLocation</span><span class="sxs-lookup"><span data-stu-id="9aa0f-162">mediaPathLocation</span></span>|<span data-ttu-id="9aa0f-163">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-163">String</span></span>| <span data-ttu-id="9aa0f-164">O datacenter usado para o caminho de mídia em uma chamada sem desvio.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-164">The datacenter used for media path in non-bypass call.</span></span>|
|<span data-ttu-id="9aa0f-165">signalingLocation</span><span class="sxs-lookup"><span data-stu-id="9aa0f-165">signalingLocation</span></span>|<span data-ttu-id="9aa0f-166">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-166">String</span></span>| <span data-ttu-id="9aa0f-167">O datacenter usado para sinalização para chamadas de bypass e não bypass.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-167">The datacenter used for signaling for both bypass and non-bypass calls.</span></span>|
|<span data-ttu-id="9aa0f-168">finalSipCode</span><span class="sxs-lookup"><span data-stu-id="9aa0f-168">finalSipCode</span></span>|<span data-ttu-id="9aa0f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="9aa0f-169">Int32</span></span>| <span data-ttu-id="9aa0f-170">O código com o qual a chamada terminou, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span><span class="sxs-lookup"><span data-stu-id="9aa0f-170">The code with which the call ended, [RFC 3261](https://tools.ietf.org/html/rfc3261).</span></span>|
|<span data-ttu-id="9aa0f-171">callEndSubReason</span><span class="sxs-lookup"><span data-stu-id="9aa0f-171">callEndSubReason</span></span>|<span data-ttu-id="9aa0f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="9aa0f-172">Int32</span></span>| <span data-ttu-id="9aa0f-173">Além dos códigos SIP, a Microsoft possui subcódigos próprios que indicam o problema específico.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-173">In addition to the SIP codes, Microsoft has own subcodes that indicate the specific issue.</span></span>|
|<span data-ttu-id="9aa0f-174">finalSipCodePhrase</span><span class="sxs-lookup"><span data-stu-id="9aa0f-174">finalSipCodePhrase</span></span>|<span data-ttu-id="9aa0f-175">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-175">String</span></span>| <span data-ttu-id="9aa0f-176">Descrição do código SIP e do subcódigo da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-176">Description of the SIP code and Microsoft subcode.</span></span>|
|<span data-ttu-id="9aa0f-177">trunkFullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="9aa0f-177">trunkFullyQualifiedDomainName</span></span>|<span data-ttu-id="9aa0f-178">String</span><span class="sxs-lookup"><span data-stu-id="9aa0f-178">String</span></span>| <span data-ttu-id="9aa0f-179">Nome de domínio totalmente qualificado do controlador de borda da sessão.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-179">Fully qualified domain name of the session border controller.</span></span>|
|<span data-ttu-id="9aa0f-180">mediaBypassEnabled</span><span class="sxs-lookup"><span data-stu-id="9aa0f-180">mediaBypassEnabled</span></span>|<span data-ttu-id="9aa0f-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9aa0f-181">Boolean</span></span>| <span data-ttu-id="9aa0f-182">Indica se o tronco foi habilitado para bypass de mídia ou não.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-182">Indicates if the trunk was enabled for media bypass or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9aa0f-183">Relações</span><span class="sxs-lookup"><span data-stu-id="9aa0f-183">Relationships</span></span>

<span data-ttu-id="9aa0f-184">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9aa0f-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9aa0f-185">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9aa0f-185">JSON representation</span></span>

<span data-ttu-id="9aa0f-186">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9aa0f-186">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
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


