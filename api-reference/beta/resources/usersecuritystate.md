---
title: tipo de recurso de userSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: dd471b06f20327eb38734276ea0562ab35db6358
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810112"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="5abb5-104">tipo de recurso de userSecurityState</span><span class="sxs-lookup"><span data-stu-id="5abb5-104">userSecurityState resource type</span></span>

 > <span data-ttu-id="5abb5-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5abb5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5abb5-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5abb5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5abb5-107">Contém informações com informações de estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="5abb5-107">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="5abb5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5abb5-108">Properties</span></span>

| <span data-ttu-id="5abb5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5abb5-109">Property</span></span>   | <span data-ttu-id="5abb5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5abb5-110">Type</span></span> |<span data-ttu-id="5abb5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5abb5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5abb5-112">aadUserId</span><span class="sxs-lookup"><span data-stu-id="5abb5-112">aadUserId</span></span>|<span data-ttu-id="5abb5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-113">String</span></span>|<span data-ttu-id="5abb5-114">Usuário AAD objeto GUID (identificador) - representa a entidade de usuário físicos/multi-account.</span><span class="sxs-lookup"><span data-stu-id="5abb5-114">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="5abb5-115">accountName</span><span class="sxs-lookup"><span data-stu-id="5abb5-115">accountName</span></span>|<span data-ttu-id="5abb5-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-116">String</span></span>|<span data-ttu-id="5abb5-117">Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="5abb5-117">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="5abb5-118">domainName</span><span class="sxs-lookup"><span data-stu-id="5abb5-118">domainName</span></span>|<span data-ttu-id="5abb5-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-119">String</span></span>|<span data-ttu-id="5abb5-120">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, o formato domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="5abb5-120">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="5abb5-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="5abb5-121">emailRole</span></span>|<span data-ttu-id="5abb5-122">emailRole</span><span class="sxs-lookup"><span data-stu-id="5abb5-122">emailRole</span></span>|<span data-ttu-id="5abb5-123">Para alertas relacionados a email - o email de uma conta de usuário 'função'.</span><span class="sxs-lookup"><span data-stu-id="5abb5-123">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="5abb5-124">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="5abb5-124">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="5abb5-125">isVpn</span><span class="sxs-lookup"><span data-stu-id="5abb5-125">isVpn</span></span>|<span data-ttu-id="5abb5-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="5abb5-126">Boolean</span></span>|<span data-ttu-id="5abb5-127">Indica se o usuário conectado por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="5abb5-127">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="5abb5-128">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="5abb5-128">logonDateTime</span></span>|<span data-ttu-id="5abb5-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5abb5-129">DateTimeOffset</span></span>|<span data-ttu-id="5abb5-130">Hora em que a entrar ocorreu.</span><span class="sxs-lookup"><span data-stu-id="5abb5-130">Time at which the sign-in occurred.</span></span> <span data-ttu-id="5abb5-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5abb5-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5abb5-132">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5abb5-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5abb5-133">identificação de logon</span><span class="sxs-lookup"><span data-stu-id="5abb5-133">logonId</span></span>|<span data-ttu-id="5abb5-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-134">String</span></span>|<span data-ttu-id="5abb5-135">ID de usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="5abb5-135">User sign-in ID.</span></span>|
|<span data-ttu-id="5abb5-136">logonIp</span><span class="sxs-lookup"><span data-stu-id="5abb5-136">logonIp</span></span>|<span data-ttu-id="5abb5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-137">String</span></span>|<span data-ttu-id="5abb5-138">Endereço IP que a solicitação de entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="5abb5-138">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="5abb5-139">logonLocation</span><span class="sxs-lookup"><span data-stu-id="5abb5-139">logonLocation</span></span>|<span data-ttu-id="5abb5-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-140">String</span></span>|<span data-ttu-id="5abb5-141">Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="5abb5-141">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="5abb5-142">logonType</span><span class="sxs-lookup"><span data-stu-id="5abb5-142">logonType</span></span>|<span data-ttu-id="5abb5-143">logonType</span><span class="sxs-lookup"><span data-stu-id="5abb5-143">logonType</span></span>|<span data-ttu-id="5abb5-144">Método do usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="5abb5-144">Method of user sign in.</span></span> <span data-ttu-id="5abb5-145">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="5abb5-145">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="5abb5-146">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="5abb5-146">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="5abb5-147">String</span><span class="sxs-lookup"><span data-stu-id="5abb5-147">String</span></span>|<span data-ttu-id="5abb5-148">Active Directory (no local) identificador de segurança (SID) do usuário.</span><span class="sxs-lookup"><span data-stu-id="5abb5-148">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="5abb5-149">riskScore</span><span class="sxs-lookup"><span data-stu-id="5abb5-149">riskScore</span></span>|<span data-ttu-id="5abb5-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-150">String</span></span>|<span data-ttu-id="5abb5-151">Pontuação de provedor gerado/calculado em risco da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="5abb5-151">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="5abb5-152">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="5abb5-152">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5abb5-153">userAccountType</span><span class="sxs-lookup"><span data-stu-id="5abb5-153">userAccountType</span></span>|<span data-ttu-id="5abb5-154">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="5abb5-154">userAccountSecurityType</span></span>|<span data-ttu-id="5abb5-155">Tipo de conta de usuário (membros do grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="5abb5-155">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="5abb5-156">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5abb5-156">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="5abb5-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5abb5-157">userPrincipalName</span></span>|<span data-ttu-id="5abb5-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5abb5-158">String</span></span>|<span data-ttu-id="5abb5-159">Entrar nome de usuário - formato da internet: (nome de conta de usuário) @(nome de domínio do DNS de conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="5abb5-159">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5abb5-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5abb5-160">JSON representation</span></span>

<span data-ttu-id="5abb5-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5abb5-161">The following is a JSON representation of the resource.</span></span>

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
