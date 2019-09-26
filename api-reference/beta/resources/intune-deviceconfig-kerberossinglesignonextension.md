---
title: tipo de recurso kerberosSingleSignOnExtension
description: Representa um perfil de extensão de logon único do tipo Kerberos.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 443ccdeac8d2249714c0cdad4af3748482acda3a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199693"
---
# <a name="kerberossinglesignonextension-resource-type"></a><span data-ttu-id="db938-103">tipo de recurso kerberosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="db938-103">kerberosSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="db938-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db938-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db938-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db938-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db938-106">Representa um perfil de extensão de logon único do tipo Kerberos.</span><span class="sxs-lookup"><span data-stu-id="db938-106">Represents a Kerberos-type Single Sign-On extension profile.</span></span>


<span data-ttu-id="db938-107">Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="db938-107">Inherits from [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db938-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db938-108">Properties</span></span>
|<span data-ttu-id="db938-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db938-109">Property</span></span>|<span data-ttu-id="db938-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="db938-110">Type</span></span>|<span data-ttu-id="db938-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="db938-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db938-112">esfera</span><span class="sxs-lookup"><span data-stu-id="db938-112">realm</span></span>|<span data-ttu-id="db938-113">String</span><span class="sxs-lookup"><span data-stu-id="db938-113">String</span></span>|<span data-ttu-id="db938-114">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="db938-114">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="db938-115">domínio</span><span class="sxs-lookup"><span data-stu-id="db938-115">domains</span></span>|<span data-ttu-id="db938-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db938-116">String collection</span></span>|<span data-ttu-id="db938-117">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="db938-117">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="db938-118">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="db938-118">blockAutomaticLogin</span></span>|<span data-ttu-id="db938-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-119">Boolean</span></span>|<span data-ttu-id="db938-120">Habilita ou desabilita o uso do chaveiro.</span><span class="sxs-lookup"><span data-stu-id="db938-120">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="db938-121">CacheName</span><span class="sxs-lookup"><span data-stu-id="db938-121">cacheName</span></span>|<span data-ttu-id="db938-122">String</span><span class="sxs-lookup"><span data-stu-id="db938-122">String</span></span>|<span data-ttu-id="db938-123">Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="db938-123">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="db938-124">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="db938-124">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="db938-125">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db938-125">String collection</span></span>|<span data-ttu-id="db938-126">Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos.</span><span class="sxs-lookup"><span data-stu-id="db938-126">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="db938-127">domainRealms</span><span class="sxs-lookup"><span data-stu-id="db938-127">domainRealms</span></span>|<span data-ttu-id="db938-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="db938-128">String collection</span></span>|<span data-ttu-id="db938-129">Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="db938-129">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="db938-130">Os territórios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="db938-130">Realms are case sensitive.</span></span>|
|<span data-ttu-id="db938-131">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="db938-131">isDefaultRealm</span></span>|<span data-ttu-id="db938-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-132">Boolean</span></span>|<span data-ttu-id="db938-133">Quando for true, o realm deste perfil será selecionado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="db938-133">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="db938-134">Necessário se vários perfis de tipo Kerberos estiverem configurados.</span><span class="sxs-lookup"><span data-stu-id="db938-134">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="db938-135">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="db938-135">passwordBlockModification</span></span>|<span data-ttu-id="db938-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-136">Boolean</span></span>|<span data-ttu-id="db938-137">Habilita ou desabilita as alterações de senha.</span><span class="sxs-lookup"><span data-stu-id="db938-137">Enables or disables password changes.</span></span>|
|<span data-ttu-id="db938-138">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="db938-138">passwordExpirationDays</span></span>|<span data-ttu-id="db938-139">Int32</span><span class="sxs-lookup"><span data-stu-id="db938-139">Int32</span></span>|<span data-ttu-id="db938-140">Substitui a expiração padrão da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="db938-140">Overrides the default password expiration in days.</span></span> <span data-ttu-id="db938-141">Para a maioria dos domínios, esse valor é calculado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="db938-141">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="db938-142">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="db938-142">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="db938-143">Int32</span><span class="sxs-lookup"><span data-stu-id="db938-143">Int32</span></span>|<span data-ttu-id="db938-144">Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15).</span><span class="sxs-lookup"><span data-stu-id="db938-144">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="db938-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="db938-145">userPrincipalName</span></span>|<span data-ttu-id="db938-146">String</span><span class="sxs-lookup"><span data-stu-id="db938-146">String</span></span>|<span data-ttu-id="db938-147">Obtém ou define o nome de usuário de princípio a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="db938-147">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="db938-148">O nome do Realm não precisa ser incluído.</span><span class="sxs-lookup"><span data-stu-id="db938-148">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="db938-149">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="db938-149">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="db938-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-150">Boolean</span></span>|<span data-ttu-id="db938-151">Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="db938-151">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="db938-152">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="db938-152">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="db938-153">Int32</span><span class="sxs-lookup"><span data-stu-id="db938-153">Int32</span></span>|<span data-ttu-id="db938-154">Obtém ou define o número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="db938-154">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="db938-155">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="db938-155">passwordMinimumLength</span></span>|<span data-ttu-id="db938-156">Int32</span><span class="sxs-lookup"><span data-stu-id="db938-156">Int32</span></span>|<span data-ttu-id="db938-157">Obtém ou define o comprimento mínimo de uma senha.</span><span class="sxs-lookup"><span data-stu-id="db938-157">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="db938-158">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="db938-158">passwordMinimumAgeDays</span></span>|<span data-ttu-id="db938-159">Int32</span><span class="sxs-lookup"><span data-stu-id="db938-159">Int32</span></span>|<span data-ttu-id="db938-160">Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.</span><span class="sxs-lookup"><span data-stu-id="db938-160">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="db938-161">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="db938-161">passwordRequirementsDescription</span></span>|<span data-ttu-id="db938-162">String</span><span class="sxs-lookup"><span data-stu-id="db938-162">String</span></span>|<span data-ttu-id="db938-163">Obtém ou define uma descrição dos requisitos de complexidade de senha.</span><span class="sxs-lookup"><span data-stu-id="db938-163">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="db938-164">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="db938-164">requireUserPresence</span></span>|<span data-ttu-id="db938-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-165">Boolean</span></span>|<span data-ttu-id="db938-166">Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain.</span><span class="sxs-lookup"><span data-stu-id="db938-166">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="db938-167">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="db938-167">activeDirectorySiteCode</span></span>|<span data-ttu-id="db938-168">String</span><span class="sxs-lookup"><span data-stu-id="db938-168">String</span></span>|<span data-ttu-id="db938-169">Obtém ou define o site do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="db938-169">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="db938-170">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="db938-170">passwordEnableLocalSync</span></span>|<span data-ttu-id="db938-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-171">Boolean</span></span>|<span data-ttu-id="db938-172">Habilita ou desabilita a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="db938-172">Enables or disables password syncing.</span></span> <span data-ttu-id="db938-173">Isso não afetará os usuários conectados com uma conta móvel no macOS.</span><span class="sxs-lookup"><span data-stu-id="db938-173">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="db938-174">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="db938-174">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="db938-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="db938-175">Boolean</span></span>|<span data-ttu-id="db938-176">Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site.</span><span class="sxs-lookup"><span data-stu-id="db938-176">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db938-177">Relações</span><span class="sxs-lookup"><span data-stu-id="db938-177">Relationships</span></span>
<span data-ttu-id="db938-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db938-178">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db938-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db938-179">JSON Representation</span></span>
<span data-ttu-id="db938-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db938-180">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.kerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.kerberosSingleSignOnExtension",
  "realm": "String",
  "domains": [
    "String"
  ],
  "blockAutomaticLogin": true,
  "cacheName": "String",
  "credentialBundleIdAccessControlList": [
    "String"
  ],
  "domainRealms": [
    "String"
  ],
  "isDefaultRealm": true,
  "passwordBlockModification": true,
  "passwordExpirationDays": 1024,
  "passwordExpirationNotificationDays": 1024,
  "userPrincipalName": "String",
  "passwordRequireActiveDirectoryComplexity": true,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumAgeDays": 1024,
  "passwordRequirementsDescription": "String",
  "requireUserPresence": true,
  "activeDirectorySiteCode": "String",
  "passwordEnableLocalSync": true,
  "blockActiveDirectorySiteAutoDiscovery": true
}
```



