---
title: tipo de recurso usersecuritystate
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67e5c7d2feb76346d754f582e34b5afe39af3d32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519509"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="6a234-104">tipo de recurso usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="6a234-104">userSecurityState resource type</span></span>

<span data-ttu-id="6a234-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a234-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a234-106">Contém informações monitoradoras sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-106">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="6a234-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a234-107">Properties</span></span>

| <span data-ttu-id="6a234-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a234-108">Property</span></span>   | <span data-ttu-id="6a234-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a234-109">Type</span></span> |<span data-ttu-id="6a234-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a234-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a234-111">aadUserId</span><span class="sxs-lookup"><span data-stu-id="6a234-111">aadUserId</span></span>|<span data-ttu-id="6a234-112">String</span><span class="sxs-lookup"><span data-stu-id="6a234-112">String</span></span>|<span data-ttu-id="6a234-113">GUID (identificador de objeto do usuário) do AAD – representa a entidade de usuário física/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="6a234-113">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="6a234-114">accountName</span><span class="sxs-lookup"><span data-stu-id="6a234-114">accountName</span></span>|<span data-ttu-id="6a234-115">String</span><span class="sxs-lookup"><span data-stu-id="6a234-115">String</span></span>|<span data-ttu-id="6a234-116">Nome da conta da conta de usuário (sem o domínio do Active Directory ou domínio DNS) `mailNickName`-(também chamado).</span><span class="sxs-lookup"><span data-stu-id="6a234-116">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="6a234-117">domainName</span><span class="sxs-lookup"><span data-stu-id="6a234-117">domainName</span></span>|<span data-ttu-id="6a234-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a234-118">String</span></span>|<span data-ttu-id="6a234-119">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="6a234-119">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="6a234-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="6a234-120">emailRole</span></span>|<span data-ttu-id="6a234-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="6a234-121">emailRole</span></span>|<span data-ttu-id="6a234-122">Para alertas relacionados a email-a função de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-122">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="6a234-123">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="6a234-123">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="6a234-124">isVpn</span><span class="sxs-lookup"><span data-stu-id="6a234-124">isVpn</span></span>|<span data-ttu-id="6a234-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a234-125">Boolean</span></span>|<span data-ttu-id="6a234-126">Indica se o usuário fez logon por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="6a234-126">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="6a234-127">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="6a234-127">logonDateTime</span></span>|<span data-ttu-id="6a234-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a234-128">DateTimeOffset</span></span>|<span data-ttu-id="6a234-129">Hora em que o logon ocorreu.</span><span class="sxs-lookup"><span data-stu-id="6a234-129">Time at which the sign-in occurred.</span></span> <span data-ttu-id="6a234-130">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6a234-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6a234-131">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6a234-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6a234-132">LogonId</span><span class="sxs-lookup"><span data-stu-id="6a234-132">logonId</span></span>|<span data-ttu-id="6a234-133">String</span><span class="sxs-lookup"><span data-stu-id="6a234-133">String</span></span>|<span data-ttu-id="6a234-134">ID de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-134">User sign-in ID.</span></span>|
|<span data-ttu-id="6a234-135">logonIp</span><span class="sxs-lookup"><span data-stu-id="6a234-135">logonIp</span></span>|<span data-ttu-id="6a234-136">String</span><span class="sxs-lookup"><span data-stu-id="6a234-136">String</span></span>|<span data-ttu-id="6a234-137">Endereço IP para o qual a solicitação de entrada originou.</span><span class="sxs-lookup"><span data-stu-id="6a234-137">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="6a234-138">logonLocation</span><span class="sxs-lookup"><span data-stu-id="6a234-138">logonLocation</span></span>|<span data-ttu-id="6a234-139">String</span><span class="sxs-lookup"><span data-stu-id="6a234-139">String</span></span>|<span data-ttu-id="6a234-140">Local (por mapeamento de endereço IP) associado a um evento de entrada do usuário por este usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-140">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="6a234-141">logonType</span><span class="sxs-lookup"><span data-stu-id="6a234-141">logonType</span></span>|<span data-ttu-id="6a234-142">logonType</span><span class="sxs-lookup"><span data-stu-id="6a234-142">logonType</span></span>|<span data-ttu-id="6a234-143">Método de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-143">Method of user sign in.</span></span> <span data-ttu-id="6a234-144">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="6a234-144">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="6a234-145">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a234-145">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="6a234-146">String</span><span class="sxs-lookup"><span data-stu-id="6a234-146">String</span></span>|<span data-ttu-id="6a234-147">O identificador de segurança (SID) do usuário do Active Directory (local).</span><span class="sxs-lookup"><span data-stu-id="6a234-147">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="6a234-148">riskScore</span><span class="sxs-lookup"><span data-stu-id="6a234-148">riskScore</span></span>|<span data-ttu-id="6a234-149">String</span><span class="sxs-lookup"><span data-stu-id="6a234-149">String</span></span>|<span data-ttu-id="6a234-150">A pontuação de risco calculado/gerado pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="6a234-150">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="6a234-151">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="6a234-151">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="6a234-152">useraccounttype</span><span class="sxs-lookup"><span data-stu-id="6a234-152">userAccountType</span></span>|<span data-ttu-id="6a234-153">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="6a234-153">userAccountSecurityType</span></span>|<span data-ttu-id="6a234-154">Tipo de conta de usuário (Associação de grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="6a234-154">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="6a234-155">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="6a234-155">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="6a234-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a234-156">userPrincipalName</span></span>|<span data-ttu-id="6a234-157">String</span><span class="sxs-lookup"><span data-stu-id="6a234-157">String</span></span>|<span data-ttu-id="6a234-158">Nome de entrada do usuário-formato da Internet: (nome da conta de usuário) @ (nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="6a234-158">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a234-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a234-159">JSON representation</span></span>

<span data-ttu-id="6a234-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a234-160">The following is a JSON representation of the resource.</span></span>

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
