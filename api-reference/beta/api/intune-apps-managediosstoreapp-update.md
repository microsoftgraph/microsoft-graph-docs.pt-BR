---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c588c0b41961aca714efc5b74f49f8421c1eb33
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984916"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="4f282-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="4f282-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="4f282-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f282-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f282-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f282-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f282-106">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f282-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f282-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f282-107">Prerequisites</span></span>
<span data-ttu-id="4f282-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f282-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f282-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f282-110">Permission type</span></span>|<span data-ttu-id="4f282-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f282-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f282-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f282-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f282-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f282-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4f282-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f282-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f282-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f282-115">Not supported.</span></span>|
|<span data-ttu-id="4f282-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f282-116">Application</span></span>|<span data-ttu-id="4f282-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f282-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f282-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f282-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4f282-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f282-119">Request headers</span></span>
|<span data-ttu-id="4f282-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f282-120">Header</span></span>|<span data-ttu-id="4f282-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4f282-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f282-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f282-122">Authorization</span></span>|<span data-ttu-id="4f282-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f282-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f282-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f282-124">Accept</span></span>|<span data-ttu-id="4f282-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f282-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f282-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f282-126">Request body</span></span>
<span data-ttu-id="4f282-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f282-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="4f282-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f282-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="4f282-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f282-129">Property</span></span>|<span data-ttu-id="4f282-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f282-130">Type</span></span>|<span data-ttu-id="4f282-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f282-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f282-132">id</span><span class="sxs-lookup"><span data-stu-id="4f282-132">id</span></span>|<span data-ttu-id="4f282-133">String</span><span class="sxs-lookup"><span data-stu-id="4f282-133">String</span></span>|<span data-ttu-id="4f282-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f282-134">Key of the entity.</span></span> <span data-ttu-id="4f282-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4f282-136">displayName</span></span>|<span data-ttu-id="4f282-137">String</span><span class="sxs-lookup"><span data-stu-id="4f282-137">String</span></span>|<span data-ttu-id="4f282-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4f282-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4f282-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-140">descrição</span><span class="sxs-lookup"><span data-stu-id="4f282-140">description</span></span>|<span data-ttu-id="4f282-141">String</span><span class="sxs-lookup"><span data-stu-id="4f282-141">String</span></span>|<span data-ttu-id="4f282-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-142">The description of the app.</span></span> <span data-ttu-id="4f282-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-144">publicador</span><span class="sxs-lookup"><span data-stu-id="4f282-144">publisher</span></span>|<span data-ttu-id="4f282-145">String</span><span class="sxs-lookup"><span data-stu-id="4f282-145">String</span></span>|<span data-ttu-id="4f282-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-146">The publisher of the app.</span></span> <span data-ttu-id="4f282-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4f282-148">largeIcon</span></span>|[<span data-ttu-id="4f282-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4f282-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4f282-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4f282-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4f282-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f282-152">createdDateTime</span></span>|<span data-ttu-id="4f282-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f282-153">DateTimeOffset</span></span>|<span data-ttu-id="4f282-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-154">The date and time the app was created.</span></span> <span data-ttu-id="4f282-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f282-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4f282-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f282-157">DateTimeOffset</span></span>|<span data-ttu-id="4f282-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4f282-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4f282-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4f282-160">isFeatured</span></span>|<span data-ttu-id="4f282-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f282-161">Boolean</span></span>|<span data-ttu-id="4f282-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4f282-163">privacyInformationUrl</span></span>|<span data-ttu-id="4f282-164">String</span><span class="sxs-lookup"><span data-stu-id="4f282-164">String</span></span>|<span data-ttu-id="4f282-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4f282-165">The privacy statement Url.</span></span> <span data-ttu-id="4f282-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4f282-167">informationUrl</span></span>|<span data-ttu-id="4f282-168">String</span><span class="sxs-lookup"><span data-stu-id="4f282-168">String</span></span>|<span data-ttu-id="4f282-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4f282-169">The more information Url.</span></span> <span data-ttu-id="4f282-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-171">owner</span><span class="sxs-lookup"><span data-stu-id="4f282-171">owner</span></span>|<span data-ttu-id="4f282-172">String</span><span class="sxs-lookup"><span data-stu-id="4f282-172">String</span></span>|<span data-ttu-id="4f282-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4f282-173">The owner of the app.</span></span> <span data-ttu-id="4f282-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-175">developer</span><span class="sxs-lookup"><span data-stu-id="4f282-175">developer</span></span>|<span data-ttu-id="4f282-176">String</span><span class="sxs-lookup"><span data-stu-id="4f282-176">String</span></span>|<span data-ttu-id="4f282-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-177">The developer of the app.</span></span> <span data-ttu-id="4f282-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-179">notes</span><span class="sxs-lookup"><span data-stu-id="4f282-179">notes</span></span>|<span data-ttu-id="4f282-180">String</span><span class="sxs-lookup"><span data-stu-id="4f282-180">String</span></span>|<span data-ttu-id="4f282-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-181">Notes for the app.</span></span> <span data-ttu-id="4f282-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4f282-183">uploadState</span></span>|<span data-ttu-id="4f282-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4f282-184">Int32</span></span>|<span data-ttu-id="4f282-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4f282-185">The upload state.</span></span> <span data-ttu-id="4f282-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4f282-187">publishingState</span></span>|[<span data-ttu-id="4f282-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4f282-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4f282-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-189">The publishing state for the app.</span></span> <span data-ttu-id="4f282-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4f282-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4f282-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f282-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4f282-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4f282-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4f282-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4f282-193">isAssigned</span></span>|<span data-ttu-id="4f282-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f282-194">Boolean</span></span>|<span data-ttu-id="4f282-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4f282-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4f282-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f282-197">roleScopeTagIds</span></span>|<span data-ttu-id="4f282-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="4f282-198">String collection</span></span>|<span data-ttu-id="4f282-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4f282-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4f282-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4f282-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4f282-201">appAvailability</span></span>|[<span data-ttu-id="4f282-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4f282-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4f282-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-203">The Application's availability.</span></span> <span data-ttu-id="4f282-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4f282-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4f282-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4f282-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4f282-206">version</span><span class="sxs-lookup"><span data-stu-id="4f282-206">version</span></span>|<span data-ttu-id="4f282-207">String</span><span class="sxs-lookup"><span data-stu-id="4f282-207">String</span></span>|<span data-ttu-id="4f282-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f282-208">The Application's version.</span></span> <span data-ttu-id="4f282-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4f282-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4f282-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="4f282-210">bundleId</span></span>|<span data-ttu-id="4f282-211">String</span><span class="sxs-lookup"><span data-stu-id="4f282-211">String</span></span>|<span data-ttu-id="4f282-212">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4f282-212">The app's Bundle ID.</span></span>|
|<span data-ttu-id="4f282-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4f282-213">appStoreUrl</span></span>|<span data-ttu-id="4f282-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f282-214">String</span></span>|<span data-ttu-id="4f282-215">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="4f282-215">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="4f282-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4f282-216">applicableDeviceType</span></span>|[<span data-ttu-id="4f282-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4f282-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4f282-218">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4f282-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4f282-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f282-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4f282-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f282-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4f282-221">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="4f282-221">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4f282-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f282-222">Response</span></span>
<span data-ttu-id="4f282-223">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f282-223">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f282-224">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f282-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f282-225">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f282-225">Request</span></span>
<span data-ttu-id="4f282-226">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f282-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="4f282-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f282-227">Response</span></span>
<span data-ttu-id="4f282-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f282-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```




