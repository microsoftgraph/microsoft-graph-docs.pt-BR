---
title: tipo de recurso de userSecurityState
description: Contém informações com informações de estado sobre a conta de usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992053"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="cea78-103">tipo de recurso de userSecurityState</span><span class="sxs-lookup"><span data-stu-id="cea78-103">userSecurityState resource type</span></span>

<span data-ttu-id="cea78-104">Contém informações com informações de estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="cea78-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="cea78-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cea78-105">Properties</span></span>

| <span data-ttu-id="cea78-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cea78-106">Property</span></span>   | <span data-ttu-id="cea78-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cea78-107">Type</span></span> |<span data-ttu-id="cea78-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cea78-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cea78-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="cea78-109">aadUserId</span></span>|<span data-ttu-id="cea78-110">String</span><span class="sxs-lookup"><span data-stu-id="cea78-110">String</span></span>|<span data-ttu-id="cea78-111">Usuário AAD objeto GUID (identificador) - representa a entidade de usuário físicos/multi-account.</span><span class="sxs-lookup"><span data-stu-id="cea78-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="cea78-112">accountName</span><span class="sxs-lookup"><span data-stu-id="cea78-112">accountName</span></span>|<span data-ttu-id="cea78-113">String</span><span class="sxs-lookup"><span data-stu-id="cea78-113">String</span></span>|<span data-ttu-id="cea78-114">Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="cea78-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="cea78-115">domainName</span><span class="sxs-lookup"><span data-stu-id="cea78-115">domainName</span></span>|<span data-ttu-id="cea78-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cea78-116">String</span></span>|<span data-ttu-id="cea78-117">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, o formato domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="cea78-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="cea78-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="cea78-118">emailRole</span></span>|<span data-ttu-id="cea78-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="cea78-119">emailRole</span></span>|<span data-ttu-id="cea78-120">Para alertas relacionados a email - o email de uma conta de usuário 'função'.</span><span class="sxs-lookup"><span data-stu-id="cea78-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="cea78-121">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="cea78-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="cea78-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="cea78-122">isVpn</span></span>|<span data-ttu-id="cea78-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="cea78-123">Boolean</span></span>|<span data-ttu-id="cea78-124">Indica se o usuário conectado por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="cea78-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="cea78-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="cea78-125">logonDateTime</span></span>|<span data-ttu-id="cea78-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cea78-126">DateTimeOffset</span></span>|<span data-ttu-id="cea78-127">Hora em que a entrar ocorreu.</span><span class="sxs-lookup"><span data-stu-id="cea78-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="cea78-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="cea78-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cea78-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cea78-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cea78-130">identificação de logon</span><span class="sxs-lookup"><span data-stu-id="cea78-130">logonId</span></span>|<span data-ttu-id="cea78-131">String</span><span class="sxs-lookup"><span data-stu-id="cea78-131">String</span></span>|<span data-ttu-id="cea78-132">ID de usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="cea78-132">User sign-in ID.</span></span>|
|<span data-ttu-id="cea78-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="cea78-133">logonIp</span></span>|<span data-ttu-id="cea78-134">String</span><span class="sxs-lookup"><span data-stu-id="cea78-134">String</span></span>|<span data-ttu-id="cea78-135">Endereço IP que a solicitação de entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="cea78-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="cea78-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="cea78-136">logonLocation</span></span>|<span data-ttu-id="cea78-137">String</span><span class="sxs-lookup"><span data-stu-id="cea78-137">String</span></span>|<span data-ttu-id="cea78-138">Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="cea78-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="cea78-139">logonType</span><span class="sxs-lookup"><span data-stu-id="cea78-139">logonType</span></span>|<span data-ttu-id="cea78-140">logonType</span><span class="sxs-lookup"><span data-stu-id="cea78-140">logonType</span></span>|<span data-ttu-id="cea78-141">Método do usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="cea78-141">Method of user sign in.</span></span> <span data-ttu-id="cea78-142">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="cea78-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="cea78-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="cea78-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="cea78-144">String</span><span class="sxs-lookup"><span data-stu-id="cea78-144">String</span></span>|<span data-ttu-id="cea78-145">Active Directory (no local) identificador de segurança (SID) do usuário.</span><span class="sxs-lookup"><span data-stu-id="cea78-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="cea78-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="cea78-146">riskScore</span></span>|<span data-ttu-id="cea78-147">String</span><span class="sxs-lookup"><span data-stu-id="cea78-147">String</span></span>|<span data-ttu-id="cea78-148">Pontuação de provedor gerado/calculado em risco da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="cea78-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="cea78-149">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="cea78-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="cea78-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="cea78-150">userAccountType</span></span>|<span data-ttu-id="cea78-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="cea78-151">userAccountSecurityType</span></span>|<span data-ttu-id="cea78-152">Tipo de conta de usuário (membros do grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="cea78-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="cea78-153">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="cea78-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="cea78-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cea78-154">userPrincipalName</span></span>|<span data-ttu-id="cea78-155">String</span><span class="sxs-lookup"><span data-stu-id="cea78-155">String</span></span>|<span data-ttu-id="cea78-156">Entrar nome de usuário - formato da internet: (nome de conta de usuário) @(nome de domínio do DNS de conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="cea78-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cea78-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cea78-157">JSON representation</span></span>

<span data-ttu-id="cea78-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cea78-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
