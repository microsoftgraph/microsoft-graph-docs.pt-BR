---
title: tipo de recurso macOSKerberosSingleSignOnExtension
description: Representa um único perfil de extensão de Sign-On de tipo Kerberos para dispositivos macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb27b51c70bc111e519cf8bb993354e638e7102d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294309"
---
# <a name="macoskerberossinglesignonextension-resource-type"></a><span data-ttu-id="e6af2-103">tipo de recurso macOSKerberosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="e6af2-103">macOSKerberosSingleSignOnExtension resource type</span></span>

<span data-ttu-id="e6af2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6af2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6af2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6af2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6af2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6af2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6af2-107">Representa um único perfil de extensão de Sign-On de tipo Kerberos para dispositivos macOS.</span><span class="sxs-lookup"><span data-stu-id="e6af2-107">Represents a Kerberos-type Single Sign-On extension profile for macOS devices.</span></span>


<span data-ttu-id="e6af2-108">Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="e6af2-108">Inherits from [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6af2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6af2-109">Properties</span></span>
|<span data-ttu-id="e6af2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6af2-110">Property</span></span>|<span data-ttu-id="e6af2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6af2-111">Type</span></span>|<span data-ttu-id="e6af2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6af2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6af2-113">esfera</span><span class="sxs-lookup"><span data-stu-id="e6af2-113">realm</span></span>|<span data-ttu-id="e6af2-114">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-114">String</span></span>|<span data-ttu-id="e6af2-115">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="e6af2-115">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="e6af2-116">domínio</span><span class="sxs-lookup"><span data-stu-id="e6af2-116">domains</span></span>|<span data-ttu-id="e6af2-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6af2-117">String collection</span></span>|<span data-ttu-id="e6af2-118">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="e6af2-118">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="e6af2-119">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="e6af2-119">blockAutomaticLogin</span></span>|<span data-ttu-id="e6af2-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-120">Boolean</span></span>|<span data-ttu-id="e6af2-121">Habilita ou desabilita o uso do chaveiro.</span><span class="sxs-lookup"><span data-stu-id="e6af2-121">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="e6af2-122">CacheName</span><span class="sxs-lookup"><span data-stu-id="e6af2-122">cacheName</span></span>|<span data-ttu-id="e6af2-123">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-123">String</span></span>|<span data-ttu-id="e6af2-124">Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="e6af2-124">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="e6af2-125">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="e6af2-125">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="e6af2-126">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6af2-126">String collection</span></span>|<span data-ttu-id="e6af2-127">Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos.</span><span class="sxs-lookup"><span data-stu-id="e6af2-127">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="e6af2-128">domainRealms</span><span class="sxs-lookup"><span data-stu-id="e6af2-128">domainRealms</span></span>|<span data-ttu-id="e6af2-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6af2-129">String collection</span></span>|<span data-ttu-id="e6af2-130">Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="e6af2-130">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="e6af2-131">Os territórios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e6af2-131">Realms are case sensitive.</span></span>|
|<span data-ttu-id="e6af2-132">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="e6af2-132">isDefaultRealm</span></span>|<span data-ttu-id="e6af2-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-133">Boolean</span></span>|<span data-ttu-id="e6af2-134">Quando for true, o realm deste perfil será selecionado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="e6af2-134">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="e6af2-135">Necessário se vários perfis de tipo Kerberos estiverem configurados.</span><span class="sxs-lookup"><span data-stu-id="e6af2-135">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="e6af2-136">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="e6af2-136">passwordBlockModification</span></span>|<span data-ttu-id="e6af2-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-137">Boolean</span></span>|<span data-ttu-id="e6af2-138">Habilita ou desabilita as alterações de senha.</span><span class="sxs-lookup"><span data-stu-id="e6af2-138">Enables or disables password changes.</span></span>|
|<span data-ttu-id="e6af2-139">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e6af2-139">passwordExpirationDays</span></span>|<span data-ttu-id="e6af2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af2-140">Int32</span></span>|<span data-ttu-id="e6af2-141">Substitui a expiração padrão da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="e6af2-141">Overrides the default password expiration in days.</span></span> <span data-ttu-id="e6af2-142">Para a maioria dos domínios, esse valor é calculado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e6af2-142">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="e6af2-143">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="e6af2-143">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="e6af2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af2-144">Int32</span></span>|<span data-ttu-id="e6af2-145">Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15).</span><span class="sxs-lookup"><span data-stu-id="e6af2-145">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="e6af2-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6af2-146">userPrincipalName</span></span>|<span data-ttu-id="e6af2-147">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-147">String</span></span>|<span data-ttu-id="e6af2-148">Obtém ou define o nome de usuário de princípio a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="e6af2-148">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="e6af2-149">O nome do Realm não precisa ser incluído.</span><span class="sxs-lookup"><span data-stu-id="e6af2-149">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="e6af2-150">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="e6af2-150">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="e6af2-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-151">Boolean</span></span>|<span data-ttu-id="e6af2-152">Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6af2-152">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="e6af2-153">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e6af2-153">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e6af2-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af2-154">Int32</span></span>|<span data-ttu-id="e6af2-155">Obtém ou define o número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e6af2-155">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="e6af2-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e6af2-156">passwordMinimumLength</span></span>|<span data-ttu-id="e6af2-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af2-157">Int32</span></span>|<span data-ttu-id="e6af2-158">Obtém ou define o comprimento mínimo de uma senha.</span><span class="sxs-lookup"><span data-stu-id="e6af2-158">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="e6af2-159">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="e6af2-159">passwordMinimumAgeDays</span></span>|<span data-ttu-id="e6af2-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e6af2-160">Int32</span></span>|<span data-ttu-id="e6af2-161">Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.</span><span class="sxs-lookup"><span data-stu-id="e6af2-161">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="e6af2-162">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="e6af2-162">passwordRequirementsDescription</span></span>|<span data-ttu-id="e6af2-163">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-163">String</span></span>|<span data-ttu-id="e6af2-164">Obtém ou define uma descrição dos requisitos de complexidade de senha.</span><span class="sxs-lookup"><span data-stu-id="e6af2-164">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="e6af2-165">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="e6af2-165">requireUserPresence</span></span>|<span data-ttu-id="e6af2-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-166">Boolean</span></span>|<span data-ttu-id="e6af2-167">Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain.</span><span class="sxs-lookup"><span data-stu-id="e6af2-167">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="e6af2-168">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="e6af2-168">activeDirectorySiteCode</span></span>|<span data-ttu-id="e6af2-169">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-169">String</span></span>|<span data-ttu-id="e6af2-170">Obtém ou define o site do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6af2-170">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="e6af2-171">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="e6af2-171">passwordEnableLocalSync</span></span>|<span data-ttu-id="e6af2-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-172">Boolean</span></span>|<span data-ttu-id="e6af2-173">Habilita ou desabilita a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="e6af2-173">Enables or disables password syncing.</span></span> <span data-ttu-id="e6af2-174">Isso não afetará os usuários conectados com uma conta móvel no macOS.</span><span class="sxs-lookup"><span data-stu-id="e6af2-174">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="e6af2-175">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="e6af2-175">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="e6af2-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6af2-176">Boolean</span></span>|<span data-ttu-id="e6af2-177">Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site.</span><span class="sxs-lookup"><span data-stu-id="e6af2-177">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="e6af2-178">passwordChangeUrl</span><span class="sxs-lookup"><span data-stu-id="e6af2-178">passwordChangeUrl</span></span>|<span data-ttu-id="e6af2-179">String</span><span class="sxs-lookup"><span data-stu-id="e6af2-179">String</span></span>|<span data-ttu-id="e6af2-180">Obtém ou define a URL para a qual o usuário será enviado quando iniciar uma alteração de senha.</span><span class="sxs-lookup"><span data-stu-id="e6af2-180">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6af2-181">Relações</span><span class="sxs-lookup"><span data-stu-id="e6af2-181">Relationships</span></span>
<span data-ttu-id="e6af2-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6af2-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6af2-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6af2-183">JSON Representation</span></span>
<span data-ttu-id="e6af2-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6af2-184">Here is a JSON representation of the resource.</span></span>
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




