---
title: tipo de recurso iosKerberosSingleSignOnExtension
description: Representa um perfil de extensão de logon único do tipo Kerberos para dispositivos iOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00da8cb6d687a8fcc828f23b0c9d78c8c38afb0b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440299"
---
# <a name="ioskerberossinglesignonextension-resource-type"></a><span data-ttu-id="ddbd8-103">tipo de recurso iosKerberosSingleSignOnExtension</span><span class="sxs-lookup"><span data-stu-id="ddbd8-103">iosKerberosSingleSignOnExtension resource type</span></span>

<span data-ttu-id="ddbd8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddbd8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ddbd8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddbd8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddbd8-107">Representa um perfil de extensão de logon único do tipo Kerberos para dispositivos iOS.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-107">Represents a Kerberos-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="ddbd8-108">Herda de [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="ddbd8-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ddbd8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ddbd8-109">Properties</span></span>
|<span data-ttu-id="ddbd8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ddbd8-110">Property</span></span>|<span data-ttu-id="ddbd8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ddbd8-111">Type</span></span>|<span data-ttu-id="ddbd8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ddbd8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddbd8-113">esfera</span><span class="sxs-lookup"><span data-stu-id="ddbd8-113">realm</span></span>|<span data-ttu-id="ddbd8-114">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-114">String</span></span>|<span data-ttu-id="ddbd8-115">Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-115">Gets or sets the case-sensitive realm name for this profile.</span></span>|
|<span data-ttu-id="ddbd8-116">domínio</span><span class="sxs-lookup"><span data-stu-id="ddbd8-116">domains</span></span>|<span data-ttu-id="ddbd8-117">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-117">String collection</span></span>|<span data-ttu-id="ddbd8-118">Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-118">Gets or sets a list of hosts or domain names for which the app extension performs SSO.</span></span>|
|<span data-ttu-id="ddbd8-119">blockAutomaticLogin</span><span class="sxs-lookup"><span data-stu-id="ddbd8-119">blockAutomaticLogin</span></span>|<span data-ttu-id="ddbd8-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-120">Boolean</span></span>|<span data-ttu-id="ddbd8-121">Habilita ou desabilita o uso do chaveiro.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-121">Enables or disables Keychain usage.</span></span>|
|<span data-ttu-id="ddbd8-122">CacheName</span><span class="sxs-lookup"><span data-stu-id="ddbd8-122">cacheName</span></span>|<span data-ttu-id="ddbd8-123">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-123">String</span></span>|<span data-ttu-id="ddbd8-124">Obtém ou define o nome genérico dos serviços de segurança do cache Kerberos a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-124">Gets or sets the Generic Security Services name of the Kerberos cache to use for this profile.</span></span>|
|<span data-ttu-id="ddbd8-125">credentialBundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="ddbd8-125">credentialBundleIdAccessControlList</span></span>|<span data-ttu-id="ddbd8-126">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-126">String collection</span></span>|<span data-ttu-id="ddbd8-127">Obtém ou define uma lista de IDs de lote de aplicativos que têm permissão para acessar o tíquete de concessão de tíquete Kerberos.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-127">Gets or sets a list of app Bundle IDs allowed to access the Kerberos Ticket Granting Ticket.</span></span>|
|<span data-ttu-id="ddbd8-128">domainRealms</span><span class="sxs-lookup"><span data-stu-id="ddbd8-128">domainRealms</span></span>|<span data-ttu-id="ddbd8-129">Coleção String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-129">String collection</span></span>|<span data-ttu-id="ddbd8-130">Obtém ou define uma lista de Realms para o mapeamento do realm do domínio personalizado.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-130">Gets or sets a list of realms for custom domain-realm mapping.</span></span> <span data-ttu-id="ddbd8-131">Os territórios diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-131">Realms are case sensitive.</span></span>|
|<span data-ttu-id="ddbd8-132">isDefaultRealm</span><span class="sxs-lookup"><span data-stu-id="ddbd8-132">isDefaultRealm</span></span>|<span data-ttu-id="ddbd8-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-133">Boolean</span></span>|<span data-ttu-id="ddbd8-134">Quando for true, o realm deste perfil será selecionado como o padrão.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-134">When true, this profile's realm will be selected as the default.</span></span> <span data-ttu-id="ddbd8-135">Necessário se vários perfis de tipo Kerberos estiverem configurados.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-135">Necessary if multiple Kerberos-type profiles are configured.</span></span>|
|<span data-ttu-id="ddbd8-136">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="ddbd8-136">passwordBlockModification</span></span>|<span data-ttu-id="ddbd8-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-137">Boolean</span></span>|<span data-ttu-id="ddbd8-138">Habilita ou desabilita as alterações de senha.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-138">Enables or disables password changes.</span></span>|
|<span data-ttu-id="ddbd8-139">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="ddbd8-139">passwordExpirationDays</span></span>|<span data-ttu-id="ddbd8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbd8-140">Int32</span></span>|<span data-ttu-id="ddbd8-141">Substitui a expiração padrão da senha em dias.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-141">Overrides the default password expiration in days.</span></span> <span data-ttu-id="ddbd8-142">Para a maioria dos domínios, esse valor é calculado automaticamente.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-142">For most domains, this value is calculated automatically.</span></span>|
|<span data-ttu-id="ddbd8-143">passwordExpirationNotificationDays</span><span class="sxs-lookup"><span data-stu-id="ddbd8-143">passwordExpirationNotificationDays</span></span>|<span data-ttu-id="ddbd8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbd8-144">Int32</span></span>|<span data-ttu-id="ddbd8-145">Obtém ou define o número de dias até que o usuário seja notificado de que sua senha irá expirar (o padrão é 15).</span><span class="sxs-lookup"><span data-stu-id="ddbd8-145">Gets or sets the number of days until the user is notified that their password will expire (default is 15).</span></span>|
|<span data-ttu-id="ddbd8-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ddbd8-146">userPrincipalName</span></span>|<span data-ttu-id="ddbd8-147">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-147">String</span></span>|<span data-ttu-id="ddbd8-148">Obtém ou define o nome de usuário de princípio a ser usado para esse perfil.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-148">Gets or sets the principle user name to use for this profile.</span></span> <span data-ttu-id="ddbd8-149">O nome do Realm não precisa ser incluído.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-149">The realm name does not need to be included.</span></span>|
|<span data-ttu-id="ddbd8-150">passwordRequireActiveDirectoryComplexity</span><span class="sxs-lookup"><span data-stu-id="ddbd8-150">passwordRequireActiveDirectoryComplexity</span></span>|<span data-ttu-id="ddbd8-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-151">Boolean</span></span>|<span data-ttu-id="ddbd8-152">Habilita ou desabilita se as senhas devem atender aos requisitos de complexidade do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-152">Enables or disables whether passwords must meet Active Directory's complexity requirements.</span></span>|
|<span data-ttu-id="ddbd8-153">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="ddbd8-153">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="ddbd8-154">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbd8-154">Int32</span></span>|<span data-ttu-id="ddbd8-155">Obtém ou define o número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-155">Gets or sets the number of previous passwords to block.</span></span>|
|<span data-ttu-id="ddbd8-156">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="ddbd8-156">passwordMinimumLength</span></span>|<span data-ttu-id="ddbd8-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbd8-157">Int32</span></span>|<span data-ttu-id="ddbd8-158">Obtém ou define o comprimento mínimo de uma senha.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-158">Gets or sets the minimum length of a password.</span></span>|
|<span data-ttu-id="ddbd8-159">passwordMinimumAgeDays</span><span class="sxs-lookup"><span data-stu-id="ddbd8-159">passwordMinimumAgeDays</span></span>|<span data-ttu-id="ddbd8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="ddbd8-160">Int32</span></span>|<span data-ttu-id="ddbd8-161">Obtém ou define o número mínimo de dias até que um usuário possa alterar sua senha novamente.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-161">Gets or sets the minimum number of days until a user can change their password again.</span></span>|
|<span data-ttu-id="ddbd8-162">passwordRequirementsDescription</span><span class="sxs-lookup"><span data-stu-id="ddbd8-162">passwordRequirementsDescription</span></span>|<span data-ttu-id="ddbd8-163">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-163">String</span></span>|<span data-ttu-id="ddbd8-164">Obtém ou define uma descrição dos requisitos de complexidade de senha.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-164">Gets or sets a description of the password complexity requirements.</span></span>|
|<span data-ttu-id="ddbd8-165">requireUserPresence</span><span class="sxs-lookup"><span data-stu-id="ddbd8-165">requireUserPresence</span></span>|<span data-ttu-id="ddbd8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-166">Boolean</span></span>|<span data-ttu-id="ddbd8-167">Obtém ou define se deve exigir autenticação por meio de ID de toque, ID de face ou uma senha para acessar a entrada de keychain.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-167">Gets or sets whether to require authentication via Touch ID, Face ID, or a passcode to access the keychain entry.</span></span>|
|<span data-ttu-id="ddbd8-168">activeDirectorySiteCode</span><span class="sxs-lookup"><span data-stu-id="ddbd8-168">activeDirectorySiteCode</span></span>|<span data-ttu-id="ddbd8-169">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-169">String</span></span>|<span data-ttu-id="ddbd8-170">Obtém ou define o site do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-170">Gets or sets the Active Directory site.</span></span>|
|<span data-ttu-id="ddbd8-171">passwordEnableLocalSync</span><span class="sxs-lookup"><span data-stu-id="ddbd8-171">passwordEnableLocalSync</span></span>|<span data-ttu-id="ddbd8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-172">Boolean</span></span>|<span data-ttu-id="ddbd8-173">Habilita ou desabilita a sincronização de senha.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-173">Enables or disables password syncing.</span></span> <span data-ttu-id="ddbd8-174">Isso não afetará os usuários conectados com uma conta móvel no macOS.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-174">This won't affect users logged in with a mobile account on macOS.</span></span>|
|<span data-ttu-id="ddbd8-175">blockActiveDirectorySiteAutoDiscovery</span><span class="sxs-lookup"><span data-stu-id="ddbd8-175">blockActiveDirectorySiteAutoDiscovery</span></span>|<span data-ttu-id="ddbd8-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ddbd8-176">Boolean</span></span>|<span data-ttu-id="ddbd8-177">Habilita ou desabilita se a extensão Kerberos pode determinar automaticamente o nome do site.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-177">Enables or disables whether the Kerberos extension can automatically determine its site name.</span></span>|
|<span data-ttu-id="ddbd8-178">passwordChangeUrl</span><span class="sxs-lookup"><span data-stu-id="ddbd8-178">passwordChangeUrl</span></span>|<span data-ttu-id="ddbd8-179">String</span><span class="sxs-lookup"><span data-stu-id="ddbd8-179">String</span></span>|<span data-ttu-id="ddbd8-180">Obtém ou define a URL para a qual o usuário será enviado quando iniciar uma alteração de senha.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-180">Gets or sets the URL that the user will be sent to when they initiate a password change.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddbd8-181">Relações</span><span class="sxs-lookup"><span data-stu-id="ddbd8-181">Relationships</span></span>
<span data-ttu-id="ddbd8-182">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ddbd8-182">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ddbd8-183">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ddbd8-183">JSON Representation</span></span>
<span data-ttu-id="ddbd8-184">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ddbd8-184">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosKerberosSingleSignOnExtension",
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



