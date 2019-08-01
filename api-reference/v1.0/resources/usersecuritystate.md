---
title: tipo de recurso usersecuritystate
description: Contém informações monitoradoras sobre a conta de usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9f5a856a9ec04eaf9a04b82e2ed7697a6735ad88
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033471"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="2b8e3-103">tipo de recurso usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="2b8e3-103">userSecurityState resource type</span></span>

<span data-ttu-id="2b8e3-104">Contém informações monitoradoras sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="2b8e3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b8e3-105">Properties</span></span>

| <span data-ttu-id="2b8e3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b8e3-106">Property</span></span>   | <span data-ttu-id="2b8e3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b8e3-107">Type</span></span> |<span data-ttu-id="2b8e3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b8e3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b8e3-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="2b8e3-109">aadUserId</span></span>|<span data-ttu-id="2b8e3-110">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-110">String</span></span>|<span data-ttu-id="2b8e3-111">GUID (identificador de objeto do usuário) do AAD – representa a entidade de usuário física/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="2b8e3-112">accountName</span><span class="sxs-lookup"><span data-stu-id="2b8e3-112">accountName</span></span>|<span data-ttu-id="2b8e3-113">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-113">String</span></span>|<span data-ttu-id="2b8e3-114">Nome da conta da conta de usuário (sem o domínio do Active Directory ou domínio DNS) `mailNickName`-(também chamado).</span><span class="sxs-lookup"><span data-stu-id="2b8e3-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="2b8e3-115">domainName</span><span class="sxs-lookup"><span data-stu-id="2b8e3-115">domainName</span></span>|<span data-ttu-id="2b8e3-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b8e3-116">String</span></span>|<span data-ttu-id="2b8e3-117">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="2b8e3-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="2b8e3-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="2b8e3-118">emailRole</span></span>|<span data-ttu-id="2b8e3-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="2b8e3-119">emailRole</span></span>|<span data-ttu-id="2b8e3-120">Para alertas relacionados a email-a função de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="2b8e3-121">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="2b8e3-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="2b8e3-122">isVpn</span></span>|<span data-ttu-id="2b8e3-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="2b8e3-123">Boolean</span></span>|<span data-ttu-id="2b8e3-124">Indica se o usuário fez logon por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="2b8e3-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="2b8e3-125">logonDateTime</span></span>|<span data-ttu-id="2b8e3-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b8e3-126">DateTimeOffset</span></span>|<span data-ttu-id="2b8e3-127">Hora em que o logon ocorreu.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="2b8e3-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2b8e3-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2b8e3-130">LogonId</span><span class="sxs-lookup"><span data-stu-id="2b8e3-130">logonId</span></span>|<span data-ttu-id="2b8e3-131">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-131">String</span></span>|<span data-ttu-id="2b8e3-132">ID de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-132">User sign-in ID.</span></span>|
|<span data-ttu-id="2b8e3-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="2b8e3-133">logonIp</span></span>|<span data-ttu-id="2b8e3-134">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-134">String</span></span>|<span data-ttu-id="2b8e3-135">Endereço IP para o qual a solicitação de entrada originou.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="2b8e3-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="2b8e3-136">logonLocation</span></span>|<span data-ttu-id="2b8e3-137">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-137">String</span></span>|<span data-ttu-id="2b8e3-138">Local (por mapeamento de endereço IP) associado a um evento de entrada do usuário por este usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="2b8e3-139">logonType</span><span class="sxs-lookup"><span data-stu-id="2b8e3-139">logonType</span></span>|<span data-ttu-id="2b8e3-140">logonType</span><span class="sxs-lookup"><span data-stu-id="2b8e3-140">logonType</span></span>|<span data-ttu-id="2b8e3-141">Método de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-141">Method of user sign in.</span></span> <span data-ttu-id="2b8e3-142">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="2b8e3-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="2b8e3-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="2b8e3-144">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-144">String</span></span>|<span data-ttu-id="2b8e3-145">O identificador de segurança (SID) do usuário do Active Directory (local).</span><span class="sxs-lookup"><span data-stu-id="2b8e3-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="2b8e3-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="2b8e3-146">riskScore</span></span>|<span data-ttu-id="2b8e3-147">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-147">String</span></span>|<span data-ttu-id="2b8e3-148">A pontuação de risco calculado/gerado pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="2b8e3-149">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="2b8e3-150">useraccounttype</span><span class="sxs-lookup"><span data-stu-id="2b8e3-150">userAccountType</span></span>|<span data-ttu-id="2b8e3-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="2b8e3-151">userAccountSecurityType</span></span>|<span data-ttu-id="2b8e3-152">Tipo de conta de usuário (Associação de grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="2b8e3-153">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="2b8e3-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2b8e3-154">userPrincipalName</span></span>|<span data-ttu-id="2b8e3-155">String</span><span class="sxs-lookup"><span data-stu-id="2b8e3-155">String</span></span>|<span data-ttu-id="2b8e3-156">Nome de entrada do usuário-formato da Internet: (nome da conta de usuário) @ (nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="2b8e3-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2b8e3-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b8e3-157">JSON representation</span></span>

<span data-ttu-id="2b8e3-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b8e3-158">The following is a JSON representation of the resource.</span></span>

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
