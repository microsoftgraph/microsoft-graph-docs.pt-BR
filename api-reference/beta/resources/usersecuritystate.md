---
title: tipo de recurso userSecuritystate
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453599"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="894fb-104">tipo de recurso userSecuritystate</span><span class="sxs-lookup"><span data-stu-id="894fb-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="894fb-105">Contém informações monitoradoras sobre a conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="894fb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="894fb-106">Properties</span></span>

| <span data-ttu-id="894fb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="894fb-107">Property</span></span>   | <span data-ttu-id="894fb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="894fb-108">Type</span></span> |<span data-ttu-id="894fb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="894fb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="894fb-110">aadUserId</span><span class="sxs-lookup"><span data-stu-id="894fb-110">aadUserId</span></span>|<span data-ttu-id="894fb-111">String</span><span class="sxs-lookup"><span data-stu-id="894fb-111">String</span></span>|<span data-ttu-id="894fb-112">GUID (identificador de objeto do usuário) do AAD – representa a entidade de usuário física/de várias contas.</span><span class="sxs-lookup"><span data-stu-id="894fb-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="894fb-113">accountName</span><span class="sxs-lookup"><span data-stu-id="894fb-113">accountName</span></span>|<span data-ttu-id="894fb-114">String</span><span class="sxs-lookup"><span data-stu-id="894fb-114">String</span></span>|<span data-ttu-id="894fb-115">Nome da conta da conta de usuário (sem o domínio do Active Directory ou domínio DNS) `mailNickName`-(também chamado).</span><span class="sxs-lookup"><span data-stu-id="894fb-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="894fb-116">domainName</span><span class="sxs-lookup"><span data-stu-id="894fb-116">domainName</span></span>|<span data-ttu-id="894fb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="894fb-117">String</span></span>|<span data-ttu-id="894fb-118">Domínio NetBIOS/Active Directory da conta de usuário (ou seja, formato de domínio \ conta).</span><span class="sxs-lookup"><span data-stu-id="894fb-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="894fb-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="894fb-119">emailRole</span></span>|<span data-ttu-id="894fb-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="894fb-120">emailRole</span></span>|<span data-ttu-id="894fb-121">Para alertas relacionados a email-a função de email da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="894fb-122">Os valores possíveis são: `unknown`, `sender`, `recipient`.</span><span class="sxs-lookup"><span data-stu-id="894fb-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="894fb-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="894fb-123">isVpn</span></span>|<span data-ttu-id="894fb-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="894fb-124">Boolean</span></span>|<span data-ttu-id="894fb-125">Indica se o usuário fez logon por meio de uma VPN.</span><span class="sxs-lookup"><span data-stu-id="894fb-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="894fb-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="894fb-126">logonDateTime</span></span>|<span data-ttu-id="894fb-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="894fb-127">DateTimeOffset</span></span>|<span data-ttu-id="894fb-128">Hora em que o logon ocorreu.</span><span class="sxs-lookup"><span data-stu-id="894fb-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="894fb-129">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="894fb-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="894fb-130">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="894fb-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="894fb-131">LogonId</span><span class="sxs-lookup"><span data-stu-id="894fb-131">logonId</span></span>|<span data-ttu-id="894fb-132">String</span><span class="sxs-lookup"><span data-stu-id="894fb-132">String</span></span>|<span data-ttu-id="894fb-133">ID de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-133">User sign-in ID.</span></span>|
|<span data-ttu-id="894fb-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="894fb-134">logonIp</span></span>|<span data-ttu-id="894fb-135">String</span><span class="sxs-lookup"><span data-stu-id="894fb-135">String</span></span>|<span data-ttu-id="894fb-136">Endereço IP para o qual a solicitação de entrada originou.</span><span class="sxs-lookup"><span data-stu-id="894fb-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="894fb-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="894fb-137">logonLocation</span></span>|<span data-ttu-id="894fb-138">String</span><span class="sxs-lookup"><span data-stu-id="894fb-138">String</span></span>|<span data-ttu-id="894fb-139">Local (por mapeamento de endereço IP) associado a um evento de entrada do usuário por este usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="894fb-140">logonType</span><span class="sxs-lookup"><span data-stu-id="894fb-140">logonType</span></span>|<span data-ttu-id="894fb-141">logonType</span><span class="sxs-lookup"><span data-stu-id="894fb-141">logonType</span></span>|<span data-ttu-id="894fb-142">Método de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-142">Method of user sign in.</span></span> <span data-ttu-id="894fb-143">Os valores possíveis são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="894fb-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="894fb-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="894fb-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="894fb-145">String</span><span class="sxs-lookup"><span data-stu-id="894fb-145">String</span></span>|<span data-ttu-id="894fb-146">O identificador de segurança (SID) do usuário do Active Directory (local).</span><span class="sxs-lookup"><span data-stu-id="894fb-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="894fb-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="894fb-147">riskScore</span></span>|<span data-ttu-id="894fb-148">String</span><span class="sxs-lookup"><span data-stu-id="894fb-148">String</span></span>|<span data-ttu-id="894fb-149">A pontuação de risco calculado/gerado pelo provedor da conta de usuário.</span><span class="sxs-lookup"><span data-stu-id="894fb-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="894fb-150">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="894fb-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="894fb-151">userAccounttype</span><span class="sxs-lookup"><span data-stu-id="894fb-151">userAccountType</span></span>|<span data-ttu-id="894fb-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="894fb-152">userAccountSecurityType</span></span>|<span data-ttu-id="894fb-153">Tipo de conta de usuário (Associação de grupo), por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="894fb-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="894fb-154">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="894fb-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="894fb-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="894fb-155">userPrincipalName</span></span>|<span data-ttu-id="894fb-156">String</span><span class="sxs-lookup"><span data-stu-id="894fb-156">String</span></span>|<span data-ttu-id="894fb-157">Nome de entrada do usuário-formato da Internet: (nome da conta de usuário) @ (nome de domínio DNS da conta de usuário).</span><span class="sxs-lookup"><span data-stu-id="894fb-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="894fb-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="894fb-158">JSON representation</span></span>

<span data-ttu-id="894fb-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="894fb-159">The following is a JSON representation of the resource.</span></span>

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
