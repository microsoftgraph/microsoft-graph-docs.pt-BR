---
title: Atualizar managedAndroidStoreApp
description: Atualiza as propriedades de um objeto managedAndroidStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75c87d098a3141feb1e6f5b235345d43313c3187
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330003"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="b08c1-103">Atualizar managedAndroidStoreApp</span><span class="sxs-lookup"><span data-stu-id="b08c1-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="b08c1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b08c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b08c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b08c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b08c1-106">Atualiza as propriedades de um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b08c1-106">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b08c1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b08c1-107">Prerequisites</span></span>
<span data-ttu-id="b08c1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b08c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b08c1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b08c1-110">Permission type</span></span>|<span data-ttu-id="b08c1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b08c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b08c1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b08c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b08c1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b08c1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b08c1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b08c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b08c1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b08c1-115">Not supported.</span></span>|
|<span data-ttu-id="b08c1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b08c1-116">Application</span></span>|<span data-ttu-id="b08c1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b08c1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b08c1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b08c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b08c1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b08c1-119">Request headers</span></span>
|<span data-ttu-id="b08c1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b08c1-120">Header</span></span>|<span data-ttu-id="b08c1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b08c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b08c1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b08c1-122">Authorization</span></span>|<span data-ttu-id="b08c1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b08c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b08c1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b08c1-124">Accept</span></span>|<span data-ttu-id="b08c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b08c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b08c1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b08c1-126">Request body</span></span>
<span data-ttu-id="b08c1-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b08c1-127">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="b08c1-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b08c1-128">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="b08c1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b08c1-129">Property</span></span>|<span data-ttu-id="b08c1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b08c1-130">Type</span></span>|<span data-ttu-id="b08c1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b08c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b08c1-132">id</span><span class="sxs-lookup"><span data-stu-id="b08c1-132">id</span></span>|<span data-ttu-id="b08c1-133">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-133">String</span></span>|<span data-ttu-id="b08c1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b08c1-134">Key of the entity.</span></span> <span data-ttu-id="b08c1-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b08c1-136">displayName</span></span>|<span data-ttu-id="b08c1-137">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-137">String</span></span>|<span data-ttu-id="b08c1-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b08c1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b08c1-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-140">descrição</span><span class="sxs-lookup"><span data-stu-id="b08c1-140">description</span></span>|<span data-ttu-id="b08c1-141">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-141">String</span></span>|<span data-ttu-id="b08c1-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-142">The description of the app.</span></span> <span data-ttu-id="b08c1-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-144">publicador</span><span class="sxs-lookup"><span data-stu-id="b08c1-144">publisher</span></span>|<span data-ttu-id="b08c1-145">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-145">String</span></span>|<span data-ttu-id="b08c1-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-146">The publisher of the app.</span></span> <span data-ttu-id="b08c1-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b08c1-148">largeIcon</span></span>|[<span data-ttu-id="b08c1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b08c1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b08c1-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b08c1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b08c1-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b08c1-152">createdDateTime</span></span>|<span data-ttu-id="b08c1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b08c1-153">DateTimeOffset</span></span>|<span data-ttu-id="b08c1-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-154">The date and time the app was created.</span></span> <span data-ttu-id="b08c1-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b08c1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b08c1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b08c1-157">DateTimeOffset</span></span>|<span data-ttu-id="b08c1-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b08c1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b08c1-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b08c1-160">isFeatured</span></span>|<span data-ttu-id="b08c1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b08c1-161">Boolean</span></span>|<span data-ttu-id="b08c1-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b08c1-163">privacyInformationUrl</span></span>|<span data-ttu-id="b08c1-164">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-164">String</span></span>|<span data-ttu-id="b08c1-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b08c1-165">The privacy statement Url.</span></span> <span data-ttu-id="b08c1-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b08c1-167">informationUrl</span></span>|<span data-ttu-id="b08c1-168">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-168">String</span></span>|<span data-ttu-id="b08c1-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b08c1-169">The more information Url.</span></span> <span data-ttu-id="b08c1-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-171">owner</span><span class="sxs-lookup"><span data-stu-id="b08c1-171">owner</span></span>|<span data-ttu-id="b08c1-172">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-172">String</span></span>|<span data-ttu-id="b08c1-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-173">The owner of the app.</span></span> <span data-ttu-id="b08c1-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-175">developer</span><span class="sxs-lookup"><span data-stu-id="b08c1-175">developer</span></span>|<span data-ttu-id="b08c1-176">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-176">String</span></span>|<span data-ttu-id="b08c1-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-177">The developer of the app.</span></span> <span data-ttu-id="b08c1-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-179">notes</span><span class="sxs-lookup"><span data-stu-id="b08c1-179">notes</span></span>|<span data-ttu-id="b08c1-180">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-180">String</span></span>|<span data-ttu-id="b08c1-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-181">Notes for the app.</span></span> <span data-ttu-id="b08c1-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b08c1-183">uploadState</span></span>|<span data-ttu-id="b08c1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b08c1-184">Int32</span></span>|<span data-ttu-id="b08c1-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="b08c1-185">The upload state.</span></span> <span data-ttu-id="b08c1-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b08c1-187">publishingState</span></span>|[<span data-ttu-id="b08c1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b08c1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b08c1-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-189">The publishing state for the app.</span></span> <span data-ttu-id="b08c1-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b08c1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b08c1-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b08c1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b08c1-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b08c1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b08c1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b08c1-193">isAssigned</span></span>|<span data-ttu-id="b08c1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b08c1-194">Boolean</span></span>|<span data-ttu-id="b08c1-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b08c1-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b08c1-197">roleScopeTagIds</span></span>|<span data-ttu-id="b08c1-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b08c1-198">String collection</span></span>|<span data-ttu-id="b08c1-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b08c1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b08c1-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b08c1-201">dependentAppCount</span></span>|<span data-ttu-id="b08c1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b08c1-202">Int32</span></span>|<span data-ttu-id="b08c1-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="b08c1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b08c1-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b08c1-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b08c1-205">appAvailability</span></span>|[<span data-ttu-id="b08c1-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b08c1-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b08c1-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-207">The Application's availability.</span></span> <span data-ttu-id="b08c1-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b08c1-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b08c1-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="b08c1-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b08c1-210">version</span><span class="sxs-lookup"><span data-stu-id="b08c1-210">version</span></span>|<span data-ttu-id="b08c1-211">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-211">String</span></span>|<span data-ttu-id="b08c1-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-212">The Application's version.</span></span> <span data-ttu-id="b08c1-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b08c1-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b08c1-214">packageId</span><span class="sxs-lookup"><span data-stu-id="b08c1-214">packageId</span></span>|<span data-ttu-id="b08c1-215">String</span><span class="sxs-lookup"><span data-stu-id="b08c1-215">String</span></span>|<span data-ttu-id="b08c1-216">A ID de pacote do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b08c1-216">The app's package ID.</span></span>|
|<span data-ttu-id="b08c1-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b08c1-217">appStoreUrl</span></span>|<span data-ttu-id="b08c1-218">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b08c1-218">String</span></span>|<span data-ttu-id="b08c1-219">A AppStoreUrl do Android.</span><span class="sxs-lookup"><span data-stu-id="b08c1-219">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="b08c1-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b08c1-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b08c1-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b08c1-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b08c1-222">O valor do sistema operacional mínimo com suporte.</span><span class="sxs-lookup"><span data-stu-id="b08c1-222">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b08c1-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="b08c1-223">Response</span></span>
<span data-ttu-id="b08c1-224">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b08c1-224">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b08c1-225">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b08c1-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="b08c1-226">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b08c1-226">Request</span></span>
<span data-ttu-id="b08c1-227">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b08c1-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="b08c1-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="b08c1-228">Response</span></span>
<span data-ttu-id="b08c1-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b08c1-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






