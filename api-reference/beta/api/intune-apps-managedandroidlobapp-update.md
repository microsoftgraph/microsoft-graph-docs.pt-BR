---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3bbc94d183afd4fb9315261dbd7bec8af871ac09
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157306"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="f2404-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="f2404-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="f2404-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2404-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2404-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f2404-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2404-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2404-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2404-107">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2404-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2404-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2404-108">Prerequisites</span></span>
<span data-ttu-id="f2404-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2404-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2404-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2404-111">Permission type</span></span>|<span data-ttu-id="f2404-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2404-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2404-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2404-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2404-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2404-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2404-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2404-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2404-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2404-116">Not supported.</span></span>|
|<span data-ttu-id="f2404-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2404-117">Application</span></span>|<span data-ttu-id="f2404-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2404-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2404-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2404-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2404-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2404-120">Request headers</span></span>
|<span data-ttu-id="f2404-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2404-121">Header</span></span>|<span data-ttu-id="f2404-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f2404-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2404-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2404-123">Authorization</span></span>|<span data-ttu-id="f2404-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2404-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2404-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2404-125">Accept</span></span>|<span data-ttu-id="f2404-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2404-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2404-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2404-127">Request body</span></span>
<span data-ttu-id="f2404-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2404-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="f2404-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2404-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="f2404-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2404-130">Property</span></span>|<span data-ttu-id="f2404-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2404-131">Type</span></span>|<span data-ttu-id="f2404-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2404-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2404-133">id</span><span class="sxs-lookup"><span data-stu-id="f2404-133">id</span></span>|<span data-ttu-id="f2404-134">String</span><span class="sxs-lookup"><span data-stu-id="f2404-134">String</span></span>|<span data-ttu-id="f2404-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f2404-135">Key of the entity.</span></span> <span data-ttu-id="f2404-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2404-137">displayName</span></span>|<span data-ttu-id="f2404-138">String</span><span class="sxs-lookup"><span data-stu-id="f2404-138">String</span></span>|<span data-ttu-id="f2404-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f2404-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2404-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-141">description</span><span class="sxs-lookup"><span data-stu-id="f2404-141">description</span></span>|<span data-ttu-id="f2404-142">String</span><span class="sxs-lookup"><span data-stu-id="f2404-142">String</span></span>|<span data-ttu-id="f2404-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-143">The description of the app.</span></span> <span data-ttu-id="f2404-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-145">publicador</span><span class="sxs-lookup"><span data-stu-id="f2404-145">publisher</span></span>|<span data-ttu-id="f2404-146">String</span><span class="sxs-lookup"><span data-stu-id="f2404-146">String</span></span>|<span data-ttu-id="f2404-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-147">The publisher of the app.</span></span> <span data-ttu-id="f2404-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2404-149">largeIcon</span></span>|[<span data-ttu-id="f2404-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2404-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2404-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f2404-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2404-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2404-153">createdDateTime</span></span>|<span data-ttu-id="f2404-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2404-154">DateTimeOffset</span></span>|<span data-ttu-id="f2404-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-155">The date and time the app was created.</span></span> <span data-ttu-id="f2404-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2404-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2404-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2404-158">DateTimeOffset</span></span>|<span data-ttu-id="f2404-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f2404-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2404-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2404-161">isFeatured</span></span>|<span data-ttu-id="f2404-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2404-162">Boolean</span></span>|<span data-ttu-id="f2404-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2404-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2404-165">String</span><span class="sxs-lookup"><span data-stu-id="f2404-165">String</span></span>|<span data-ttu-id="f2404-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f2404-166">The privacy statement Url.</span></span> <span data-ttu-id="f2404-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2404-168">informationUrl</span></span>|<span data-ttu-id="f2404-169">String</span><span class="sxs-lookup"><span data-stu-id="f2404-169">String</span></span>|<span data-ttu-id="f2404-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f2404-170">The more information Url.</span></span> <span data-ttu-id="f2404-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2404-172">owner</span></span>|<span data-ttu-id="f2404-173">String</span><span class="sxs-lookup"><span data-stu-id="f2404-173">String</span></span>|<span data-ttu-id="f2404-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f2404-174">The owner of the app.</span></span> <span data-ttu-id="f2404-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2404-176">developer</span></span>|<span data-ttu-id="f2404-177">String</span><span class="sxs-lookup"><span data-stu-id="f2404-177">String</span></span>|<span data-ttu-id="f2404-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-178">The developer of the app.</span></span> <span data-ttu-id="f2404-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2404-180">notes</span></span>|<span data-ttu-id="f2404-181">String</span><span class="sxs-lookup"><span data-stu-id="f2404-181">String</span></span>|<span data-ttu-id="f2404-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-182">Notes for the app.</span></span> <span data-ttu-id="f2404-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2404-184">uploadState</span></span>|<span data-ttu-id="f2404-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2404-185">Int32</span></span>|<span data-ttu-id="f2404-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f2404-186">The upload state.</span></span> <span data-ttu-id="f2404-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="f2404-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="f2404-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2404-189">publishingState</span></span>|[<span data-ttu-id="f2404-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2404-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2404-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-191">The publishing state for the app.</span></span> <span data-ttu-id="f2404-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f2404-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2404-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2404-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="f2404-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f2404-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2404-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f2404-195">isAssigned</span></span>|<span data-ttu-id="f2404-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2404-196">Boolean</span></span>|<span data-ttu-id="f2404-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="f2404-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f2404-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f2404-199">roleScopeTagIds</span></span>|<span data-ttu-id="f2404-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2404-200">String collection</span></span>|<span data-ttu-id="f2404-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="f2404-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f2404-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f2404-203">dependentAppCount</span></span>|<span data-ttu-id="f2404-204">Int32</span><span class="sxs-lookup"><span data-stu-id="f2404-204">Int32</span></span>|<span data-ttu-id="f2404-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="f2404-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f2404-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="f2404-207">supersedingAppCount</span></span>|<span data-ttu-id="f2404-208">Int32</span><span class="sxs-lookup"><span data-stu-id="f2404-208">Int32</span></span>|<span data-ttu-id="f2404-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="f2404-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="f2404-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="f2404-211">supersededAppCount</span></span>|<span data-ttu-id="f2404-212">Int32</span><span class="sxs-lookup"><span data-stu-id="f2404-212">Int32</span></span>|<span data-ttu-id="f2404-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="f2404-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="f2404-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="f2404-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f2404-215">appAvailability</span></span>|[<span data-ttu-id="f2404-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f2404-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f2404-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-217">The Application's availability.</span></span> <span data-ttu-id="f2404-218">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f2404-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f2404-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f2404-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f2404-220">version</span><span class="sxs-lookup"><span data-stu-id="f2404-220">version</span></span>|<span data-ttu-id="f2404-221">String</span><span class="sxs-lookup"><span data-stu-id="f2404-221">String</span></span>|<span data-ttu-id="f2404-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2404-222">The Application's version.</span></span> <span data-ttu-id="f2404-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f2404-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f2404-224">committedContentVersion</span></span>|<span data-ttu-id="f2404-225">String</span><span class="sxs-lookup"><span data-stu-id="f2404-225">String</span></span>|<span data-ttu-id="f2404-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f2404-226">The internal committed content version.</span></span> <span data-ttu-id="f2404-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f2404-228">fileName</span><span class="sxs-lookup"><span data-stu-id="f2404-228">fileName</span></span>|<span data-ttu-id="f2404-229">String</span><span class="sxs-lookup"><span data-stu-id="f2404-229">String</span></span>|<span data-ttu-id="f2404-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f2404-230">The name of the main Lob application file.</span></span> <span data-ttu-id="f2404-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f2404-232">size</span><span class="sxs-lookup"><span data-stu-id="f2404-232">size</span></span>|<span data-ttu-id="f2404-233">Int64</span><span class="sxs-lookup"><span data-stu-id="f2404-233">Int64</span></span>|<span data-ttu-id="f2404-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f2404-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="f2404-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2404-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f2404-236">packageId</span><span class="sxs-lookup"><span data-stu-id="f2404-236">packageId</span></span>|<span data-ttu-id="f2404-237">String</span><span class="sxs-lookup"><span data-stu-id="f2404-237">String</span></span>|<span data-ttu-id="f2404-238">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="f2404-238">The package identifier.</span></span>|
|<span data-ttu-id="f2404-239">identityName</span><span class="sxs-lookup"><span data-stu-id="f2404-239">identityName</span></span>|<span data-ttu-id="f2404-240">String</span><span class="sxs-lookup"><span data-stu-id="f2404-240">String</span></span>|<span data-ttu-id="f2404-241">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f2404-241">The Identity Name.</span></span>|
|<span data-ttu-id="f2404-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2404-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2404-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2404-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f2404-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f2404-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f2404-245">versionName</span><span class="sxs-lookup"><span data-stu-id="f2404-245">versionName</span></span>|<span data-ttu-id="f2404-246">String</span><span class="sxs-lookup"><span data-stu-id="f2404-246">String</span></span>|<span data-ttu-id="f2404-247">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f2404-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2404-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="f2404-248">versionCode</span></span>|<span data-ttu-id="f2404-249">String</span><span class="sxs-lookup"><span data-stu-id="f2404-249">String</span></span>|<span data-ttu-id="f2404-250">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f2404-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f2404-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f2404-251">identityVersion</span></span>|<span data-ttu-id="f2404-252">String</span><span class="sxs-lookup"><span data-stu-id="f2404-252">String</span></span>|<span data-ttu-id="f2404-253">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f2404-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f2404-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2404-254">Response</span></span>
<span data-ttu-id="f2404-255">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2404-255">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2404-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2404-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2404-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2404-257">Request</span></span>
<span data-ttu-id="f2404-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2404-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1588

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f2404-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2404-259">Response</span></span>
<span data-ttu-id="f2404-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2404-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1760

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




