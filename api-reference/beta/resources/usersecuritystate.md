---
title: tipo de recurso de userSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517236"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="3ffef-104">tipo de recurso de userSecurityState</span><span class="sxs-lookup"><span data-stu-id="3ffef-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ffef-105">Contém informações com informações de estado sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3ffef-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="3ffef-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ffef-106">Properties</span></span>

| <span data-ttu-id="3ffef-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ffef-107">Property</span></span>   | <span data-ttu-id="3ffef-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ffef-108">Type</span></span> |<span data-ttu-id="3ffef-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ffef-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ffef-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="3ffef-110">aadUserId</span></span>|<span data-ttu-id="3ffef-111">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-111">String</span></span>|<span data-ttu-id="3ffef-112">Usuário AAD objeto GUID (identificador) - representa a entidade de usuário físicos/multi-account.</span><span class="sxs-lookup"><span data-stu-id="3ffef-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="3ffef-113">accountName</span><span class="sxs-lookup"><span data-stu-id="3ffef-113">accountName</span></span>|<span data-ttu-id="3ffef-114">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-114">String</span></span>|<span data-ttu-id="3ffef-115">Nome da conta de usuário (sem o domínio do Active Directory ou domínio DNS) - conta (também chamado de `mailNickName`).</span><span class="sxs-lookup"><span data-stu-id="3ffef-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="3ffef-116">domainName</span><span class="sxs-lookup"><span data-stu-id="3ffef-116">domainName</span></span>|<span data-ttu-id="3ffef-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ffef-117">String</span></span>|<span data-ttu-id="3ffef-118">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, o formato domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="3ffef-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="3ffef-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="3ffef-119">emailRole</span></span>|<span data-ttu-id="3ffef-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="3ffef-120">emailRole</span></span>|<span data-ttu-id="3ffef-121">Para alertas relacionados a email - o email de uma conta de usuário 'função'.</span><span class="sxs-lookup"><span data-stu-id="3ffef-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="3ffef-122">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="3ffef-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="3ffef-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="3ffef-123">isVpn</span></span>|<span data-ttu-id="3ffef-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3ffef-124">Boolean</span></span>|<span data-ttu-id="3ffef-125">Indica se o usuário conectado por meio da VPN.</span><span class="sxs-lookup"><span data-stu-id="3ffef-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="3ffef-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffef-126">logonDateTime</span></span>|<span data-ttu-id="3ffef-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffef-127">DateTimeOffset</span></span>|<span data-ttu-id="3ffef-128">Hora em que a entrar ocorreu.</span><span class="sxs-lookup"><span data-stu-id="3ffef-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="3ffef-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3ffef-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ffef-130">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ffef-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3ffef-131">identificação de logon</span><span class="sxs-lookup"><span data-stu-id="3ffef-131">logonId</span></span>|<span data-ttu-id="3ffef-132">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-132">String</span></span>|<span data-ttu-id="3ffef-133">ID de usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="3ffef-133">User sign-in ID.</span></span>|
|<span data-ttu-id="3ffef-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="3ffef-134">logonIp</span></span>|<span data-ttu-id="3ffef-135">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-135">String</span></span>|<span data-ttu-id="3ffef-136">Endereço IP que a solicitação de entrada se originou.</span><span class="sxs-lookup"><span data-stu-id="3ffef-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="3ffef-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="3ffef-137">logonLocation</span></span>|<span data-ttu-id="3ffef-138">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-138">String</span></span>|<span data-ttu-id="3ffef-139">Local (por um mapeamento de endereço IP) associado a um evento de entrada do usuário por esse usuário.</span><span class="sxs-lookup"><span data-stu-id="3ffef-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="3ffef-140">logonType</span><span class="sxs-lookup"><span data-stu-id="3ffef-140">logonType</span></span>|<span data-ttu-id="3ffef-141">logonType</span><span class="sxs-lookup"><span data-stu-id="3ffef-141">logonType</span></span>|<span data-ttu-id="3ffef-142">Método do usuário entrar.</span><span class="sxs-lookup"><span data-stu-id="3ffef-142">Method of user sign in.</span></span> <span data-ttu-id="3ffef-143">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="3ffef-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="3ffef-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="3ffef-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="3ffef-145">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-145">String</span></span>|<span data-ttu-id="3ffef-146">Active Directory (no local) identificador de segurança (SID) do usuário.</span><span class="sxs-lookup"><span data-stu-id="3ffef-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="3ffef-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="3ffef-147">riskScore</span></span>|<span data-ttu-id="3ffef-148">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-148">String</span></span>|<span data-ttu-id="3ffef-149">Pontuação de provedor gerado/calculado em risco da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="3ffef-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="3ffef-150">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="3ffef-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="3ffef-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="3ffef-151">userAccountType</span></span>|<span data-ttu-id="3ffef-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="3ffef-152">userAccountSecurityType</span></span>|<span data-ttu-id="3ffef-153">Tipo de conta de usuário (membros do grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="3ffef-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="3ffef-154">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="3ffef-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="3ffef-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3ffef-155">userPrincipalName</span></span>|<span data-ttu-id="3ffef-156">String</span><span class="sxs-lookup"><span data-stu-id="3ffef-156">String</span></span>|<span data-ttu-id="3ffef-157">Entrar nome de usuário - formato da internet: (nome de conta de usuário) @(nome de domínio do DNS de conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="3ffef-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ffef-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ffef-158">JSON representation</span></span>

<span data-ttu-id="3ffef-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ffef-159">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
