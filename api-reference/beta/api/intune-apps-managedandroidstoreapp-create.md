---
title: Criar managedAndroidStoreApp
description: Cria um novo objeto managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 566ceaa4818f335b2f98ba0b3c86a5895f5d96df
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935759"
---
# <a name="create-managedandroidstoreapp"></a><span data-ttu-id="7ef72-103">Criar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="7ef72-103">Create managedAndroidStoreApp</span></span>

> <span data-ttu-id="7ef72-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ef72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ef72-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ef72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ef72-106">Cria um novo objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ef72-106">Create a new [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ef72-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7ef72-107">Prerequisites</span></span>
<span data-ttu-id="7ef72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef72-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7ef72-110">Permission type</span></span>|<span data-ttu-id="7ef72-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7ef72-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ef72-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7ef72-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ef72-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef72-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ef72-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7ef72-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ef72-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ef72-115">Not supported.</span></span>|
|<span data-ttu-id="7ef72-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7ef72-116">Application</span></span>|<span data-ttu-id="7ef72-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7ef72-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ef72-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7ef72-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7ef72-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef72-119">Request headers</span></span>
|<span data-ttu-id="7ef72-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7ef72-120">Header</span></span>|<span data-ttu-id="7ef72-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7ef72-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ef72-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7ef72-122">Authorization</span></span>|<span data-ttu-id="7ef72-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7ef72-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ef72-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7ef72-124">Accept</span></span>|<span data-ttu-id="7ef72-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ef72-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ef72-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef72-126">Request body</span></span>
<span data-ttu-id="7ef72-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="7ef72-127">In the request body, supply a JSON representation for the managedAndroidStoreApp object.</span></span>

<span data-ttu-id="7ef72-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="7ef72-128">The following table shows the properties that are required when you create the managedAndroidStoreApp.</span></span>

|<span data-ttu-id="7ef72-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ef72-129">Property</span></span>|<span data-ttu-id="7ef72-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ef72-130">Type</span></span>|<span data-ttu-id="7ef72-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ef72-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ef72-132">id</span><span class="sxs-lookup"><span data-stu-id="7ef72-132">id</span></span>|<span data-ttu-id="7ef72-133">String</span><span class="sxs-lookup"><span data-stu-id="7ef72-133">String</span></span>|<span data-ttu-id="7ef72-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7ef72-134">Key of the entity.</span></span> <span data-ttu-id="7ef72-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7ef72-136">displayName</span></span>|<span data-ttu-id="7ef72-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-137">String</span></span>|<span data-ttu-id="7ef72-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="7ef72-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7ef72-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-140">description</span><span class="sxs-lookup"><span data-stu-id="7ef72-140">description</span></span>|<span data-ttu-id="7ef72-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-141">String</span></span>|<span data-ttu-id="7ef72-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-142">The description of the app.</span></span> <span data-ttu-id="7ef72-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-144">publicador</span><span class="sxs-lookup"><span data-stu-id="7ef72-144">publisher</span></span>|<span data-ttu-id="7ef72-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-145">String</span></span>|<span data-ttu-id="7ef72-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-146">The publisher of the app.</span></span> <span data-ttu-id="7ef72-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7ef72-148">largeIcon</span></span>|[<span data-ttu-id="7ef72-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7ef72-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7ef72-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="7ef72-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7ef72-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef72-152">createdDateTime</span></span>|<span data-ttu-id="7ef72-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef72-153">DateTimeOffset</span></span>|<span data-ttu-id="7ef72-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-154">The date and time the app was created.</span></span> <span data-ttu-id="7ef72-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7ef72-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7ef72-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ef72-157">DateTimeOffset</span></span>|<span data-ttu-id="7ef72-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="7ef72-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7ef72-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7ef72-160">isFeatured</span></span>|<span data-ttu-id="7ef72-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ef72-161">Boolean</span></span>|<span data-ttu-id="7ef72-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7ef72-163">privacyInformationUrl</span></span>|<span data-ttu-id="7ef72-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-164">String</span></span>|<span data-ttu-id="7ef72-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="7ef72-165">The privacy statement Url.</span></span> <span data-ttu-id="7ef72-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7ef72-167">informationUrl</span></span>|<span data-ttu-id="7ef72-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-168">String</span></span>|<span data-ttu-id="7ef72-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="7ef72-169">The more information Url.</span></span> <span data-ttu-id="7ef72-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-171">owner</span><span class="sxs-lookup"><span data-stu-id="7ef72-171">owner</span></span>|<span data-ttu-id="7ef72-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-172">String</span></span>|<span data-ttu-id="7ef72-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-173">The owner of the app.</span></span> <span data-ttu-id="7ef72-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-175">developer</span><span class="sxs-lookup"><span data-stu-id="7ef72-175">developer</span></span>|<span data-ttu-id="7ef72-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-176">String</span></span>|<span data-ttu-id="7ef72-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-177">The developer of the app.</span></span> <span data-ttu-id="7ef72-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-179">notes</span><span class="sxs-lookup"><span data-stu-id="7ef72-179">notes</span></span>|<span data-ttu-id="7ef72-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-180">String</span></span>|<span data-ttu-id="7ef72-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-181">Notes for the app.</span></span> <span data-ttu-id="7ef72-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7ef72-183">uploadState</span></span>|<span data-ttu-id="7ef72-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7ef72-184">Int32</span></span>|<span data-ttu-id="7ef72-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="7ef72-185">The upload state.</span></span> <span data-ttu-id="7ef72-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7ef72-187">publishingState</span></span>|[<span data-ttu-id="7ef72-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7ef72-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7ef72-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-189">The publishing state for the app.</span></span> <span data-ttu-id="7ef72-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="7ef72-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7ef72-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ef72-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7ef72-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="7ef72-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7ef72-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7ef72-193">isAssigned</span></span>|<span data-ttu-id="7ef72-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ef72-194">Boolean</span></span>|<span data-ttu-id="7ef72-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7ef72-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7ef72-197">roleScopeTagIds</span></span>|<span data-ttu-id="7ef72-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-198">String collection</span></span>|<span data-ttu-id="7ef72-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="7ef72-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7ef72-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7ef72-201">dependentAppCount</span></span>|<span data-ttu-id="7ef72-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7ef72-202">Int32</span></span>|<span data-ttu-id="7ef72-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="7ef72-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7ef72-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7ef72-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="7ef72-205">appAvailability</span></span>|[<span data-ttu-id="7ef72-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="7ef72-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="7ef72-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-207">The Application's availability.</span></span> <span data-ttu-id="7ef72-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7ef72-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="7ef72-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="7ef72-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="7ef72-210">version</span><span class="sxs-lookup"><span data-stu-id="7ef72-210">version</span></span>|<span data-ttu-id="7ef72-211">String</span><span class="sxs-lookup"><span data-stu-id="7ef72-211">String</span></span>|<span data-ttu-id="7ef72-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-212">The Application's version.</span></span> <span data-ttu-id="7ef72-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7ef72-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="7ef72-214">packageId</span><span class="sxs-lookup"><span data-stu-id="7ef72-214">packageId</span></span>|<span data-ttu-id="7ef72-215">String</span><span class="sxs-lookup"><span data-stu-id="7ef72-215">String</span></span>|<span data-ttu-id="7ef72-216">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7ef72-216">The app's package ID.</span></span>|
|<span data-ttu-id="7ef72-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7ef72-217">appStoreUrl</span></span>|<span data-ttu-id="7ef72-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ef72-218">String</span></span>|<span data-ttu-id="7ef72-219">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="7ef72-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="7ef72-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ef72-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7ef72-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ef72-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7ef72-222">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="7ef72-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7ef72-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ef72-223">Response</span></span>
<span data-ttu-id="7ef72-224">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7ef72-224">If successful, this method returns a `201 Created` response code and a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ef72-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7ef72-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ef72-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7ef72-226">Request</span></span>
<span data-ttu-id="7ef72-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7ef72-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="7ef72-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="7ef72-228">Response</span></span>
<span data-ttu-id="7ef72-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7ef72-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```




