---
title: Tipo de recurso userSecurityState
description: Contém informações de estado sobre a conta de usuário.
localization_priority: Normal
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edd3f3eeb4e8efffde9abd4a8fb53a8a5ddb9ea3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722255"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="b1321-103">Tipo de recurso userSecurityState</span><span class="sxs-lookup"><span data-stu-id="b1321-103">userSecurityState resource type</span></span>

<span data-ttu-id="b1321-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1321-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1321-105">Contém informações de estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="b1321-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1321-106">Properties</span></span>

| <span data-ttu-id="b1321-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1321-107">Property</span></span>   | <span data-ttu-id="b1321-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1321-108">Type</span></span> |<span data-ttu-id="b1321-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1321-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b1321-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="b1321-110">aadUserId</span></span>|<span data-ttu-id="b1321-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-111">String</span></span>|<span data-ttu-id="b1321-112">Identificador de objeto do usuário AAD (GUID) - representa a entidade de usuário físico/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="b1321-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="b1321-113">accountName</span><span class="sxs-lookup"><span data-stu-id="b1321-113">accountName</span></span>|<span data-ttu-id="b1321-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-114">String</span></span>|<span data-ttu-id="b1321-115">Nome da conta de usuário (sem domínio do Active Directory ou domínio DNS) - (também chamado `mailNickName` ).</span><span class="sxs-lookup"><span data-stu-id="b1321-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="b1321-116">domainName</span><span class="sxs-lookup"><span data-stu-id="b1321-116">domainName</span></span>|<span data-ttu-id="b1321-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-117">String</span></span>|<span data-ttu-id="b1321-118">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio\conta).</span><span class="sxs-lookup"><span data-stu-id="b1321-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="b1321-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="b1321-119">emailRole</span></span>|<span data-ttu-id="b1321-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="b1321-120">emailRole</span></span>|<span data-ttu-id="b1321-121">Para alertas relacionados a email - 'função' de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="b1321-122">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="b1321-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="b1321-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="b1321-123">isVpn</span></span>|<span data-ttu-id="b1321-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1321-124">Boolean</span></span>|<span data-ttu-id="b1321-125">Indica se o usuário fez logons por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="b1321-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="b1321-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="b1321-126">logonDateTime</span></span>|<span data-ttu-id="b1321-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1321-127">DateTimeOffset</span></span>|<span data-ttu-id="b1321-128">Hora em que ocorreu a login.</span><span class="sxs-lookup"><span data-stu-id="b1321-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="b1321-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b1321-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b1321-130">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b1321-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="b1321-131">logonId</span><span class="sxs-lookup"><span data-stu-id="b1321-131">logonId</span></span>|<span data-ttu-id="b1321-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-132">String</span></span>|<span data-ttu-id="b1321-133">ID de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-133">User sign-in ID.</span></span>|
|<span data-ttu-id="b1321-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="b1321-134">logonIp</span></span>|<span data-ttu-id="b1321-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-135">String</span></span>|<span data-ttu-id="b1321-136">Endereço IP da solicitação de login originada.</span><span class="sxs-lookup"><span data-stu-id="b1321-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="b1321-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="b1321-137">logonLocation</span></span>|<span data-ttu-id="b1321-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-138">String</span></span>|<span data-ttu-id="b1321-139">Local (por mapeamento de endereço IP) associado a um evento de login do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="b1321-140">logonType</span><span class="sxs-lookup"><span data-stu-id="b1321-140">logonType</span></span>|<span data-ttu-id="b1321-141">logonType</span><span class="sxs-lookup"><span data-stu-id="b1321-141">logonType</span></span>|<span data-ttu-id="b1321-142">Método de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-142">Method of user sign in.</span></span> <span data-ttu-id="b1321-143">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="b1321-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="b1321-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1321-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="b1321-145">String</span><span class="sxs-lookup"><span data-stu-id="b1321-145">String</span></span>|<span data-ttu-id="b1321-146">Identificador de Segurança (SID) do Active Directory (local) do usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="b1321-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="b1321-147">riskScore</span></span>|<span data-ttu-id="b1321-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-148">String</span></span>|<span data-ttu-id="b1321-149">Pontuação de risco gerada/calculada pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="b1321-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="b1321-150">Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="b1321-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="b1321-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="b1321-151">userAccountType</span></span>|<span data-ttu-id="b1321-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="b1321-152">userAccountSecurityType</span></span>|<span data-ttu-id="b1321-153">Tipo de conta de usuário (associação ao grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="b1321-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="b1321-154">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="b1321-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="b1321-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1321-155">userPrincipalName</span></span>|<span data-ttu-id="b1321-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1321-156">String</span></span>|<span data-ttu-id="b1321-157">Nome de login do usuário - formato da Internet: (nome da conta de usuário)@(nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="b1321-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1321-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1321-158">JSON representation</span></span>

<span data-ttu-id="b1321-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1321-159">The following is a JSON representation of the resource.</span></span>

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


