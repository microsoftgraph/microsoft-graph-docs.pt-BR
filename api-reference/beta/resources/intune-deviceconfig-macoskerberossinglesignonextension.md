---
title: tipo de recurso macOSKerberosSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos macOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd43b26ba310cc9d25d719bdcae683b4f1716b41
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636697"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a><span data-ttu-id="16519-103">tipo de recurso macOSKerberosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="16519-103">macOSKerberosSingleSignOnExtension resource type</span></span>

> <span data-ttu-id="16519-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16519-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16519-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16519-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16519-106">Representa um perfil de extensão de logon único de tipo Kerberos para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="16519-106">Represents a Kerberos-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="16519-107">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="16519-107">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16519-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16519-108">Properties</span></span>
|<span data-ttu-id="16519-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16519-109">Property</span></span>|<span data-ttu-id="16519-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="16519-110">Type</span></span>|<span data-ttu-id="16519-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="16519-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16519-112">esfera</span><span class="sxs-lookup"><span data-stu-id="16519-112">realm</span></span>|<span data-ttu-id="16519-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-113">String</span></span>|<span data-ttu-id="16519-114">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="16519-114">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="16519-115">domínio</span><span class="sxs-lookup"><span data-stu-id="16519-115">domains</span></span>|<span data-ttu-id="16519-116">String collection</span><span class="sxs-lookup"><span data-stu-id="16519-116">String collection</span></span>|<span data-ttu-id="16519-117">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="16519-117">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="16519-118">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="16519-118">blockAutomaticLogin</span></span>|<span data-ttu-id="16519-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-119">Boolean</span></span>|<span data-ttu-id="16519-120">Habilita ou desabilita o uso do chaveiro.</span><span class="sxs-lookup"><span data-stu-id="16519-120">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="16519-121">CacheName</span><span class="sxs-lookup"><span data-stu-id="16519-121">cacheName</span></span>|<span data-ttu-id="16519-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-122">String</span></span>|<span data-ttu-id="16519-123">Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="16519-123">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="16519-124">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="16519-124">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="16519-125">String collection</span><span class="sxs-lookup"><span data-stu-id="16519-125">String collection</span></span>|<span data-ttu-id="16519-126">Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos.</span><span class="sxs-lookup"><span data-stu-id="16519-126">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="16519-127">domainRealms</span><span class="sxs-lookup"><span data-stu-id="16519-127">domainRealms</span></span>|<span data-ttu-id="16519-128">String collection</span><span class="sxs-lookup"><span data-stu-id="16519-128">String collection</span></span>|<span data-ttu-id="16519-129">Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="16519-129">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="16519-130">Os territórios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="16519-130">Realms are case sensitive.</span></span>|
|<span data-ttu-id="16519-131">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="16519-131">isDefaultRealm</span></span>|<span data-ttu-id="16519-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-132">Boolean</span></span>|<span data-ttu-id="16519-133">Quando for true, o realm deste perfil será selecionado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="16519-133">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="16519-134">Necessário se vários perfis de tipo Kerberos estiverem configurados.</span><span class="sxs-lookup"><span data-stu-id="16519-134">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="16519-135">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="16519-135">passwordBlockModification</span></span>|<span data-ttu-id="16519-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-136">Boolean</span></span>|<span data-ttu-id="16519-137">Habilita ou desabilita as alterações de senha.</span><span class="sxs-lookup"><span data-stu-id="16519-137">Enables or disables password changes.</span></span>|
|<span data-ttu-id="16519-138">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="16519-138">passwordExpirationDays</span></span>|<span data-ttu-id="16519-139">Int32</span><span class="sxs-lookup"><span data-stu-id="16519-139">Int32</span></span>|<span data-ttu-id="16519-140">Substitui a expiração padrão da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="16519-140">Overrides the default password expiration in days.</span></span> <span data-ttu-id="16519-141">Para a maioria dos domínios, esse valor é calculado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="16519-141">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="16519-142">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="16519-142">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="16519-143">Int32</span><span class="sxs-lookup"><span data-stu-id="16519-143">Int32</span></span>|<span data-ttu-id="16519-144">Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15).</span><span class="sxs-lookup"><span data-stu-id="16519-144">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="16519-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16519-145">userPrincipalName</span></span>|<span data-ttu-id="16519-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-146">String</span></span>|<span data-ttu-id="16519-147">Obtém ou define o nome de usuário de princípio a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="16519-147">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="16519-148">O nome do Realm não precisa ser incluído.</span><span class="sxs-lookup"><span data-stu-id="16519-148">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="16519-149">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="16519-149">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="16519-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-150">Boolean</span></span>|<span data-ttu-id="16519-151">Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16519-151">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="16519-152">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="16519-152">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="16519-153">Int32</span><span class="sxs-lookup"><span data-stu-id="16519-153">Int32</span></span>|<span data-ttu-id="16519-154">Obtém ou define o número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="16519-154">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="16519-155">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="16519-155">passwordMinimumLength</span></span>|<span data-ttu-id="16519-156">Int32</span><span class="sxs-lookup"><span data-stu-id="16519-156">Int32</span></span>|<span data-ttu-id="16519-157">Obtém ou define o comprimento mínimo de uma senha.</span><span class="sxs-lookup"><span data-stu-id="16519-157">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="16519-158">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="16519-158">passwordMinimumAgeDays</span></span>|<span data-ttu-id="16519-159">Int32</span><span class="sxs-lookup"><span data-stu-id="16519-159">Int32</span></span>|<span data-ttu-id="16519-160">Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.</span><span class="sxs-lookup"><span data-stu-id="16519-160">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="16519-161">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="16519-161">passwordRequirementsDescription</span></span>|<span data-ttu-id="16519-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-162">String</span></span>|<span data-ttu-id="16519-163">Obtém ou define uma descrição dos requisitos de complexidade de senha.</span><span class="sxs-lookup"><span data-stu-id="16519-163">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="16519-164">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="16519-164">requireUserPresence</span></span>|<span data-ttu-id="16519-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-165">Boolean</span></span>|<span data-ttu-id="16519-166">Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain.</span><span class="sxs-lookup"><span data-stu-id="16519-166">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="16519-167">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="16519-167">activeDirectorySiteCode</span></span>|<span data-ttu-id="16519-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-168">String</span></span>|<span data-ttu-id="16519-169">Obtém ou define o site do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="16519-169">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="16519-170">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="16519-170">passwordEnableLocalSync</span></span>|<span data-ttu-id="16519-171">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-171">Boolean</span></span>|<span data-ttu-id="16519-172">Habilita ou desabilita a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="16519-172">Enables or disables password syncing.</span></span> <span data-ttu-id="16519-173">Isso não afetará os usuários conectados com uma conta móvel no macOS.</span><span class="sxs-lookup"><span data-stu-id="16519-173">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="16519-174">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="16519-174">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="16519-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="16519-175">Boolean</span></span>|<span data-ttu-id="16519-176">Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site.</span><span class="sxs-lookup"><span data-stu-id="16519-176">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="16519-177">passwordChangeUrl</span><span class="sxs-lookup"><span data-stu-id="16519-177">passwordChangeUrl</span></span>|<span data-ttu-id="16519-178">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16519-178">String</span></span>|<span data-ttu-id="16519-179">Obtém ou define a URL para a qual o usuário será enviado quando iniciar uma alteração de senha.</span><span class="sxs-lookup"><span data-stu-id="16519-179">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16519-180">Relações</span><span class="sxs-lookup"><span data-stu-id="16519-180">Relationships</span></span>
<span data-ttu-id="16519-181">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16519-181">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16519-182">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16519-182">JSON Representation</span></span>
<span data-ttu-id="16519-183">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16519-183">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKerberosSingleSignOnExtension",
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
  "blockActiveDirectorySiteAutoDiscovery": true,
  "passwordChangeUrl": "String"
}
```



