---
title: Tipo de recurso userSecurityState
description: Contém informações de estado sobre a conta de usuário.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c95f898a729138a7af88eaf25fa4cbc0c5fc9bb9
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761776"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="3df40-103">Tipo de recurso userSecurityState</span><span class="sxs-lookup"><span data-stu-id="3df40-103">userSecurityState resource type</span></span>

<span data-ttu-id="3df40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3df40-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3df40-105">Contém informações de estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="3df40-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3df40-106">Properties</span></span>

| <span data-ttu-id="3df40-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3df40-107">Property</span></span>   | <span data-ttu-id="3df40-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3df40-108">Type</span></span> |<span data-ttu-id="3df40-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3df40-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3df40-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="3df40-110">aadUserId</span></span>|<span data-ttu-id="3df40-111">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-111">String</span></span>|<span data-ttu-id="3df40-112">Identificador de objeto do usuário AAD (GUID) - representa a entidade de usuário físico/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="3df40-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="3df40-113">accountName</span><span class="sxs-lookup"><span data-stu-id="3df40-113">accountName</span></span>|<span data-ttu-id="3df40-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-114">String</span></span>|<span data-ttu-id="3df40-115">Nome da conta de usuário (sem domínio do Active Directory ou domínio DNS) - (também chamado `mailNickName` ).</span><span class="sxs-lookup"><span data-stu-id="3df40-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="3df40-116">domainName</span><span class="sxs-lookup"><span data-stu-id="3df40-116">domainName</span></span>|<span data-ttu-id="3df40-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-117">String</span></span>|<span data-ttu-id="3df40-118">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio\conta).</span><span class="sxs-lookup"><span data-stu-id="3df40-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="3df40-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="3df40-119">emailRole</span></span>|<span data-ttu-id="3df40-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="3df40-120">emailRole</span></span>|<span data-ttu-id="3df40-121">Para alertas relacionados a email - 'função' de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="3df40-122">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="3df40-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="3df40-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="3df40-123">isVpn</span></span>|<span data-ttu-id="3df40-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="3df40-124">Boolean</span></span>|<span data-ttu-id="3df40-125">Indica se o usuário fez logons por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="3df40-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="3df40-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="3df40-126">logonDateTime</span></span>|<span data-ttu-id="3df40-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3df40-127">DateTimeOffset</span></span>|<span data-ttu-id="3df40-128">Hora em que ocorreu a login.</span><span class="sxs-lookup"><span data-stu-id="3df40-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="3df40-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3df40-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3df40-130">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="3df40-130">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="3df40-131">logonId</span><span class="sxs-lookup"><span data-stu-id="3df40-131">logonId</span></span>|<span data-ttu-id="3df40-132">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-132">String</span></span>|<span data-ttu-id="3df40-133">ID de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-133">User sign-in ID.</span></span>|
|<span data-ttu-id="3df40-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="3df40-134">logonIp</span></span>|<span data-ttu-id="3df40-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-135">String</span></span>|<span data-ttu-id="3df40-136">Endereço IP da solicitação de login originada.</span><span class="sxs-lookup"><span data-stu-id="3df40-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="3df40-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="3df40-137">logonLocation</span></span>|<span data-ttu-id="3df40-138">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-138">String</span></span>|<span data-ttu-id="3df40-139">Local (por mapeamento de endereço IP) associado a um evento de login do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="3df40-140">logonType</span><span class="sxs-lookup"><span data-stu-id="3df40-140">logonType</span></span>|<span data-ttu-id="3df40-141">logonType</span><span class="sxs-lookup"><span data-stu-id="3df40-141">logonType</span></span>|<span data-ttu-id="3df40-142">Método de login do usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-142">Method of user sign in.</span></span> <span data-ttu-id="3df40-143">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="3df40-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="3df40-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="3df40-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="3df40-145">String</span><span class="sxs-lookup"><span data-stu-id="3df40-145">String</span></span>|<span data-ttu-id="3df40-146">Identificador de Segurança (SID) do Active Directory (local) do usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="3df40-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="3df40-147">riskScore</span></span>|<span data-ttu-id="3df40-148">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-148">String</span></span>|<span data-ttu-id="3df40-149">Pontuação de risco gerada/calculada pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3df40-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="3df40-150">Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="3df40-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="3df40-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="3df40-151">userAccountType</span></span>|<span data-ttu-id="3df40-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="3df40-152">userAccountSecurityType</span></span>|<span data-ttu-id="3df40-153">Tipo de conta de usuário (associação ao grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="3df40-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="3df40-154">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="3df40-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="3df40-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3df40-155">userPrincipalName</span></span>|<span data-ttu-id="3df40-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3df40-156">String</span></span>|<span data-ttu-id="3df40-157">Nome de login do usuário - formato da Internet: (nome da conta de usuário)@(nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="3df40-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3df40-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3df40-158">JSON representation</span></span>

<span data-ttu-id="3df40-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3df40-159">The following is a JSON representation of the resource.</span></span>

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


