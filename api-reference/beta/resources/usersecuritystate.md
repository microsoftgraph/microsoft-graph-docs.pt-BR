---
title: tipo de recurso usersecuritystate
description: Contém informações monitoradoras sobre a conta de usuário.
localization_priority: Normal
author: krbain
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55c7a55678f4120a7e3c1755a599fcde36ffcd5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057812"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="e15f5-103">tipo de recurso usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="e15f5-103">userSecurityState resource type</span></span>

<span data-ttu-id="e15f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e15f5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e15f5-105">Contém informações monitoradoras sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="e15f5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e15f5-106">Properties</span></span>

| <span data-ttu-id="e15f5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e15f5-107">Property</span></span>   | <span data-ttu-id="e15f5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e15f5-108">Type</span></span> |<span data-ttu-id="e15f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e15f5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e15f5-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="e15f5-110">aadUserId</span></span>|<span data-ttu-id="e15f5-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-111">String</span></span>|<span data-ttu-id="e15f5-112">GUID (identificador de objeto do usuário) do AAD – representa a entidade de usuário física/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="e15f5-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="e15f5-113">accountName</span><span class="sxs-lookup"><span data-stu-id="e15f5-113">accountName</span></span>|<span data-ttu-id="e15f5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-114">String</span></span>|<span data-ttu-id="e15f5-115">Nome da conta da conta de usuário (sem o domínio do Active Directory ou domínio DNS)-(também chamado `mailNickName` ).</span><span class="sxs-lookup"><span data-stu-id="e15f5-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="e15f5-116">domainName</span><span class="sxs-lookup"><span data-stu-id="e15f5-116">domainName</span></span>|<span data-ttu-id="e15f5-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-117">String</span></span>|<span data-ttu-id="e15f5-118">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="e15f5-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="e15f5-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="e15f5-119">emailRole</span></span>|<span data-ttu-id="e15f5-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="e15f5-120">emailRole</span></span>|<span data-ttu-id="e15f5-121">Para alertas relacionados a email-a função de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="e15f5-122">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="e15f5-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="e15f5-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="e15f5-123">isVpn</span></span>|<span data-ttu-id="e15f5-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="e15f5-124">Boolean</span></span>|<span data-ttu-id="e15f5-125">Indica se o usuário fez logon por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="e15f5-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="e15f5-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="e15f5-126">logonDateTime</span></span>|<span data-ttu-id="e15f5-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e15f5-127">DateTimeOffset</span></span>|<span data-ttu-id="e15f5-128">Hora em que o logon ocorreu.</span><span class="sxs-lookup"><span data-stu-id="e15f5-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="e15f5-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e15f5-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e15f5-130">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e15f5-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e15f5-131">LogonId</span><span class="sxs-lookup"><span data-stu-id="e15f5-131">logonId</span></span>|<span data-ttu-id="e15f5-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-132">String</span></span>|<span data-ttu-id="e15f5-133">ID de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-133">User sign-in ID.</span></span>|
|<span data-ttu-id="e15f5-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="e15f5-134">logonIp</span></span>|<span data-ttu-id="e15f5-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-135">String</span></span>|<span data-ttu-id="e15f5-136">Endereço IP para o qual a solicitação de entrada originou.</span><span class="sxs-lookup"><span data-stu-id="e15f5-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="e15f5-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="e15f5-137">logonLocation</span></span>|<span data-ttu-id="e15f5-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-138">String</span></span>|<span data-ttu-id="e15f5-139">Local (por mapeamento de endereço IP) associado a um evento de entrada do usuário por este usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="e15f5-140">logonType</span><span class="sxs-lookup"><span data-stu-id="e15f5-140">logonType</span></span>|<span data-ttu-id="e15f5-141">logonType</span><span class="sxs-lookup"><span data-stu-id="e15f5-141">logonType</span></span>|<span data-ttu-id="e15f5-142">Método de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-142">Method of user sign in.</span></span> <span data-ttu-id="e15f5-143">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="e15f5-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="e15f5-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e15f5-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="e15f5-145">String</span><span class="sxs-lookup"><span data-stu-id="e15f5-145">String</span></span>|<span data-ttu-id="e15f5-146">O identificador de segurança (SID) do usuário do Active Directory (local).</span><span class="sxs-lookup"><span data-stu-id="e15f5-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="e15f5-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="e15f5-147">riskScore</span></span>|<span data-ttu-id="e15f5-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-148">String</span></span>|<span data-ttu-id="e15f5-149">A pontuação de risco calculado/gerado pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="e15f5-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="e15f5-150">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="e15f5-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="e15f5-151">useraccounttype</span><span class="sxs-lookup"><span data-stu-id="e15f5-151">userAccountType</span></span>|<span data-ttu-id="e15f5-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="e15f5-152">userAccountSecurityType</span></span>|<span data-ttu-id="e15f5-153">Tipo de conta de usuário (Associação de grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="e15f5-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="e15f5-154">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e15f5-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e15f5-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e15f5-155">userPrincipalName</span></span>|<span data-ttu-id="e15f5-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e15f5-156">String</span></span>|<span data-ttu-id="e15f5-157">Nome de entrada do usuário-formato da Internet: (nome da conta de usuário) @ (nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="e15f5-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e15f5-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e15f5-158">JSON representation</span></span>

<span data-ttu-id="e15f5-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e15f5-159">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


