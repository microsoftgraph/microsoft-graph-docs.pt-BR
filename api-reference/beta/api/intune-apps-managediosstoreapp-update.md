---
title: Atualizar managedIOSStoreApp
description: Atualiza as propriedades de um objeto managedIOSStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5f4b41a276896c0a8ef6de18e7ee010799954a2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405543"
---
# <a name="update-managediosstoreapp"></a><span data-ttu-id="0f854-103">Atualizar managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="0f854-103">Update managedIOSStoreApp</span></span>

<span data-ttu-id="0f854-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f854-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f854-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f854-107">Atualiza as propriedades de um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f854-107">Update the properties of a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f854-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0f854-108">Prerequisites</span></span>
<span data-ttu-id="0f854-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f854-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0f854-111">Permission type</span></span>|<span data-ttu-id="0f854-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0f854-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f854-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0f854-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0f854-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f854-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f854-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0f854-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f854-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0f854-116">Not supported.</span></span>|
|<span data-ttu-id="0f854-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0f854-117">Application</span></span>|<span data-ttu-id="0f854-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f854-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f854-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0f854-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0f854-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0f854-120">Request headers</span></span>
|<span data-ttu-id="0f854-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0f854-121">Header</span></span>|<span data-ttu-id="0f854-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0f854-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f854-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0f854-123">Authorization</span></span>|<span data-ttu-id="0f854-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f854-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f854-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0f854-125">Accept</span></span>|<span data-ttu-id="0f854-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0f854-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f854-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0f854-127">Request body</span></span>
<span data-ttu-id="0f854-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f854-128">In the request body, supply a JSON representation for the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>

<span data-ttu-id="0f854-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f854-129">The following table shows the properties that are required when you create the [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md).</span></span>

|<span data-ttu-id="0f854-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f854-130">Property</span></span>|<span data-ttu-id="0f854-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f854-131">Type</span></span>|<span data-ttu-id="0f854-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f854-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f854-133">id</span><span class="sxs-lookup"><span data-stu-id="0f854-133">id</span></span>|<span data-ttu-id="0f854-134">String</span><span class="sxs-lookup"><span data-stu-id="0f854-134">String</span></span>|<span data-ttu-id="0f854-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0f854-135">Key of the entity.</span></span> <span data-ttu-id="0f854-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0f854-137">displayName</span></span>|<span data-ttu-id="0f854-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f854-138">String</span></span>|<span data-ttu-id="0f854-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0f854-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f854-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-141">description</span><span class="sxs-lookup"><span data-stu-id="0f854-141">description</span></span>|<span data-ttu-id="0f854-142">String</span><span class="sxs-lookup"><span data-stu-id="0f854-142">String</span></span>|<span data-ttu-id="0f854-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-143">The description of the app.</span></span> <span data-ttu-id="0f854-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-145">publicador</span><span class="sxs-lookup"><span data-stu-id="0f854-145">publisher</span></span>|<span data-ttu-id="0f854-146">String</span><span class="sxs-lookup"><span data-stu-id="0f854-146">String</span></span>|<span data-ttu-id="0f854-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-147">The publisher of the app.</span></span> <span data-ttu-id="0f854-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f854-149">largeIcon</span></span>|[<span data-ttu-id="0f854-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f854-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f854-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="0f854-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f854-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f854-153">createdDateTime</span></span>|<span data-ttu-id="0f854-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f854-154">DateTimeOffset</span></span>|<span data-ttu-id="0f854-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-155">The date and time the app was created.</span></span> <span data-ttu-id="0f854-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f854-157">lastModifiedDateTime</span></span>|<span data-ttu-id="0f854-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f854-158">DateTimeOffset</span></span>|<span data-ttu-id="0f854-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0f854-159">The date and time the app was last modified.</span></span> <span data-ttu-id="0f854-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f854-161">isFeatured</span></span>|<span data-ttu-id="0f854-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f854-162">Boolean</span></span>|<span data-ttu-id="0f854-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f854-164">privacyInformationUrl</span></span>|<span data-ttu-id="0f854-165">String</span><span class="sxs-lookup"><span data-stu-id="0f854-165">String</span></span>|<span data-ttu-id="0f854-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="0f854-166">The privacy statement Url.</span></span> <span data-ttu-id="0f854-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f854-168">informationUrl</span></span>|<span data-ttu-id="0f854-169">String</span><span class="sxs-lookup"><span data-stu-id="0f854-169">String</span></span>|<span data-ttu-id="0f854-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0f854-170">The more information Url.</span></span> <span data-ttu-id="0f854-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-172">owner</span><span class="sxs-lookup"><span data-stu-id="0f854-172">owner</span></span>|<span data-ttu-id="0f854-173">String</span><span class="sxs-lookup"><span data-stu-id="0f854-173">String</span></span>|<span data-ttu-id="0f854-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="0f854-174">The owner of the app.</span></span> <span data-ttu-id="0f854-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-176">developer</span><span class="sxs-lookup"><span data-stu-id="0f854-176">developer</span></span>|<span data-ttu-id="0f854-177">String</span><span class="sxs-lookup"><span data-stu-id="0f854-177">String</span></span>|<span data-ttu-id="0f854-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-178">The developer of the app.</span></span> <span data-ttu-id="0f854-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-180">notes</span><span class="sxs-lookup"><span data-stu-id="0f854-180">notes</span></span>|<span data-ttu-id="0f854-181">String</span><span class="sxs-lookup"><span data-stu-id="0f854-181">String</span></span>|<span data-ttu-id="0f854-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-182">Notes for the app.</span></span> <span data-ttu-id="0f854-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f854-184">uploadState</span></span>|<span data-ttu-id="0f854-185">Int32</span><span class="sxs-lookup"><span data-stu-id="0f854-185">Int32</span></span>|<span data-ttu-id="0f854-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="0f854-186">The upload state.</span></span> <span data-ttu-id="0f854-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f854-188">publishingState</span></span>|[<span data-ttu-id="0f854-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0f854-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f854-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-190">The publishing state for the app.</span></span> <span data-ttu-id="0f854-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="0f854-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f854-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f854-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0f854-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0f854-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f854-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f854-194">isAssigned</span></span>|<span data-ttu-id="0f854-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f854-195">Boolean</span></span>|<span data-ttu-id="0f854-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="0f854-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f854-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f854-198">roleScopeTagIds</span></span>|<span data-ttu-id="0f854-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="0f854-199">String collection</span></span>|<span data-ttu-id="0f854-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0f854-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f854-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0f854-202">dependentAppCount</span></span>|<span data-ttu-id="0f854-203">Int32</span><span class="sxs-lookup"><span data-stu-id="0f854-203">Int32</span></span>|<span data-ttu-id="0f854-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="0f854-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0f854-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0f854-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="0f854-206">appAvailability</span></span>|[<span data-ttu-id="0f854-207">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="0f854-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="0f854-208">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-208">The Application's availability.</span></span> <span data-ttu-id="0f854-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="0f854-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="0f854-210">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="0f854-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="0f854-211">version</span><span class="sxs-lookup"><span data-stu-id="0f854-211">version</span></span>|<span data-ttu-id="0f854-212">String</span><span class="sxs-lookup"><span data-stu-id="0f854-212">String</span></span>|<span data-ttu-id="0f854-213">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f854-213">The Application's version.</span></span> <span data-ttu-id="0f854-214">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0f854-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="0f854-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="0f854-215">bundleId</span></span>|<span data-ttu-id="0f854-216">String</span><span class="sxs-lookup"><span data-stu-id="0f854-216">String</span></span>|<span data-ttu-id="0f854-217">A ID do pacote de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0f854-217">The app's Bundle ID.</span></span>|
|<span data-ttu-id="0f854-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0f854-218">appStoreUrl</span></span>|<span data-ttu-id="0f854-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f854-219">String</span></span>|<span data-ttu-id="0f854-220">A AppStoreUrl da Apple.</span><span class="sxs-lookup"><span data-stu-id="0f854-220">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="0f854-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="0f854-221">applicableDeviceType</span></span>|[<span data-ttu-id="0f854-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="0f854-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="0f854-223">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="0f854-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="0f854-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f854-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0f854-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0f854-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="0f854-226">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="0f854-226">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0f854-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f854-227">Response</span></span>
<span data-ttu-id="0f854-228">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0f854-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f854-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0f854-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f854-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0f854-230">Request</span></span>
<span data-ttu-id="0f854-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0f854-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1238

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
    "v12_0": true,
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="0f854-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="0f854-232">Response</span></span>
<span data-ttu-id="0f854-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0f854-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1410

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
    "v12_0": true,
    "v13_0": true
  }
}
```



