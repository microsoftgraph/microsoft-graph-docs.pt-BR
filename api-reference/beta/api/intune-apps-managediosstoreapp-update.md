---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04968a462522ad69840512caf78ea3a52aafec1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974453"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="4b173-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="4b173-103">Update managedIOSStoreApp</span></span>

> <span data-ttu-id="4b173-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4b173-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b173-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4b173-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b173-106">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b173-106">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b173-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4b173-107">Prerequisites</span></span>
<span data-ttu-id="4b173-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b173-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b173-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b173-110">Permission type</span></span>|<span data-ttu-id="4b173-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4b173-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b173-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b173-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b173-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b173-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4b173-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b173-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b173-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b173-115">Not supported.</span></span>|
|<span data-ttu-id="4b173-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b173-116">Application</span></span>|<span data-ttu-id="4b173-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b173-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b173-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b173-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4b173-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b173-119">Request headers</span></span>
|<span data-ttu-id="4b173-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4b173-120">Header</span></span>|<span data-ttu-id="4b173-121">Valor</span><span class="sxs-lookup"><span data-stu-id="4b173-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b173-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b173-122">Authorization</span></span>|<span data-ttu-id="4b173-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b173-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b173-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4b173-124">Accept</span></span>|<span data-ttu-id="4b173-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b173-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b173-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b173-126">Request body</span></span>
<span data-ttu-id="4b173-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b173-127">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="4b173-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b173-128">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="4b173-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b173-129">Property</span></span>|<span data-ttu-id="4b173-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b173-130">Type</span></span>|<span data-ttu-id="4b173-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b173-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b173-132">id</span><span class="sxs-lookup"><span data-stu-id="4b173-132">id</span></span>|<span data-ttu-id="4b173-133">String</span><span class="sxs-lookup"><span data-stu-id="4b173-133">String</span></span>|<span data-ttu-id="4b173-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4b173-134">Key of the entity.</span></span> <span data-ttu-id="4b173-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b173-136">displayName</span></span>|<span data-ttu-id="4b173-137">String</span><span class="sxs-lookup"><span data-stu-id="4b173-137">String</span></span>|<span data-ttu-id="4b173-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4b173-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4b173-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-140">descrição</span><span class="sxs-lookup"><span data-stu-id="4b173-140">description</span></span>|<span data-ttu-id="4b173-141">String</span><span class="sxs-lookup"><span data-stu-id="4b173-141">String</span></span>|<span data-ttu-id="4b173-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-142">The description of the app.</span></span> <span data-ttu-id="4b173-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-144">publicador</span><span class="sxs-lookup"><span data-stu-id="4b173-144">publisher</span></span>|<span data-ttu-id="4b173-145">String</span><span class="sxs-lookup"><span data-stu-id="4b173-145">String</span></span>|<span data-ttu-id="4b173-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-146">The publisher of the app.</span></span> <span data-ttu-id="4b173-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4b173-148">largeIcon</span></span>|[<span data-ttu-id="4b173-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4b173-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4b173-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4b173-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4b173-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b173-152">createdDateTime</span></span>|<span data-ttu-id="4b173-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b173-153">DateTimeOffset</span></span>|<span data-ttu-id="4b173-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-154">The date and time the app was created.</span></span> <span data-ttu-id="4b173-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b173-156">lastModifiedDateTime</span></span>|<span data-ttu-id="4b173-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b173-157">DateTimeOffset</span></span>|<span data-ttu-id="4b173-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4b173-158">The date and time the app was last modified.</span></span> <span data-ttu-id="4b173-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4b173-160">isFeatured</span></span>|<span data-ttu-id="4b173-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b173-161">Boolean</span></span>|<span data-ttu-id="4b173-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4b173-163">privacyInformationUrl</span></span>|<span data-ttu-id="4b173-164">String</span><span class="sxs-lookup"><span data-stu-id="4b173-164">String</span></span>|<span data-ttu-id="4b173-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4b173-165">The privacy statement Url.</span></span> <span data-ttu-id="4b173-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4b173-167">informationUrl</span></span>|<span data-ttu-id="4b173-168">String</span><span class="sxs-lookup"><span data-stu-id="4b173-168">String</span></span>|<span data-ttu-id="4b173-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4b173-169">The more information Url.</span></span> <span data-ttu-id="4b173-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-171">owner</span><span class="sxs-lookup"><span data-stu-id="4b173-171">owner</span></span>|<span data-ttu-id="4b173-172">String</span><span class="sxs-lookup"><span data-stu-id="4b173-172">String</span></span>|<span data-ttu-id="4b173-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4b173-173">The owner of the app.</span></span> <span data-ttu-id="4b173-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-175">developer</span><span class="sxs-lookup"><span data-stu-id="4b173-175">developer</span></span>|<span data-ttu-id="4b173-176">String</span><span class="sxs-lookup"><span data-stu-id="4b173-176">String</span></span>|<span data-ttu-id="4b173-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-177">The developer of the app.</span></span> <span data-ttu-id="4b173-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-179">notes</span><span class="sxs-lookup"><span data-stu-id="4b173-179">notes</span></span>|<span data-ttu-id="4b173-180">String</span><span class="sxs-lookup"><span data-stu-id="4b173-180">String</span></span>|<span data-ttu-id="4b173-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-181">Notes for the app.</span></span> <span data-ttu-id="4b173-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="4b173-183">uploadState</span></span>|<span data-ttu-id="4b173-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4b173-184">Int32</span></span>|<span data-ttu-id="4b173-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="4b173-185">The upload state.</span></span> <span data-ttu-id="4b173-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="4b173-187">publishingState</span></span>|[<span data-ttu-id="4b173-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4b173-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4b173-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-189">The publishing state for the app.</span></span> <span data-ttu-id="4b173-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4b173-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4b173-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b173-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4b173-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4b173-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4b173-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4b173-193">isAssigned</span></span>|<span data-ttu-id="4b173-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b173-194">Boolean</span></span>|<span data-ttu-id="4b173-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4b173-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4b173-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4b173-197">roleScopeTagIds</span></span>|<span data-ttu-id="4b173-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b173-198">String collection</span></span>|<span data-ttu-id="4b173-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4b173-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4b173-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4b173-201">dependentAppCount</span></span>|<span data-ttu-id="4b173-202">Int32</span><span class="sxs-lookup"><span data-stu-id="4b173-202">Int32</span></span>|<span data-ttu-id="4b173-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="4b173-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4b173-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4b173-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4b173-205">appAvailability</span></span>|[<span data-ttu-id="4b173-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4b173-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4b173-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-207">The Application's availability.</span></span> <span data-ttu-id="4b173-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4b173-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4b173-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="4b173-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4b173-210">version</span><span class="sxs-lookup"><span data-stu-id="4b173-210">version</span></span>|<span data-ttu-id="4b173-211">String</span><span class="sxs-lookup"><span data-stu-id="4b173-211">String</span></span>|<span data-ttu-id="4b173-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4b173-212">The Application's version.</span></span> <span data-ttu-id="4b173-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="4b173-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4b173-214">bundleId</span><span class="sxs-lookup"><span data-stu-id="4b173-214">bundleId</span></span>|<span data-ttu-id="4b173-215">String</span><span class="sxs-lookup"><span data-stu-id="4b173-215">String</span></span>|<span data-ttu-id="4b173-216">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4b173-216">The app's Bundle ID.</span></span>|
|<span data-ttu-id="4b173-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="4b173-217">appStoreUrl</span></span>|<span data-ttu-id="4b173-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4b173-218">String</span></span>|<span data-ttu-id="4b173-219">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="4b173-219">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="4b173-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4b173-220">applicableDeviceType</span></span>|[<span data-ttu-id="4b173-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4b173-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4b173-222">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4b173-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4b173-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b173-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4b173-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4b173-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4b173-225">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="4b173-225">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="4b173-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b173-226">Response</span></span>
<span data-ttu-id="4b173-227">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b173-227">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b173-228">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b173-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b173-229">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b173-229">Request</span></span>
<span data-ttu-id="4b173-230">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b173-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1218

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="4b173-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b173-231">Response</span></span>
<span data-ttu-id="4b173-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4b173-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1390

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
  "dependentAppCount": 1,
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





