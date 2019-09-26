---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17de78d0c4b90e31cd2a575521b05bfe28c31072
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173189"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="6c84d-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="6c84d-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="6c84d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c84d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c84d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c84d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c84d-106">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c84d-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c84d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c84d-107">Prerequisites</span></span>
<span data-ttu-id="6c84d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c84d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c84d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c84d-110">Permission type</span></span>|<span data-ttu-id="6c84d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c84d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c84d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c84d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c84d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c84d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c84d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c84d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c84d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c84d-115">Not supported.</span></span>|
|<span data-ttu-id="6c84d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c84d-116">Application</span></span>|<span data-ttu-id="6c84d-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c84d-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c84d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c84d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6c84d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c84d-119">Request headers</span></span>
|<span data-ttu-id="6c84d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c84d-120">Header</span></span>|<span data-ttu-id="6c84d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c84d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c84d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c84d-122">Authorization</span></span>|<span data-ttu-id="6c84d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c84d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c84d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c84d-124">Accept</span></span>|<span data-ttu-id="6c84d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c84d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c84d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c84d-126">Request body</span></span>
<span data-ttu-id="6c84d-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c84d-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="6c84d-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c84d-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="6c84d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c84d-129">Property</span></span>|<span data-ttu-id="6c84d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c84d-130">Type</span></span>|<span data-ttu-id="6c84d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c84d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c84d-132">id</span><span class="sxs-lookup"><span data-stu-id="6c84d-132">id</span></span>|<span data-ttu-id="6c84d-133">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-133">String</span></span>|<span data-ttu-id="6c84d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c84d-134">Key of the entity.</span></span> <span data-ttu-id="6c84d-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c84d-136">displayName</span></span>|<span data-ttu-id="6c84d-137">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-137">String</span></span>|<span data-ttu-id="6c84d-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6c84d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6c84d-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-140">descrição</span><span class="sxs-lookup"><span data-stu-id="6c84d-140">description</span></span>|<span data-ttu-id="6c84d-141">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-141">String</span></span>|<span data-ttu-id="6c84d-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-142">The description of the app.</span></span> <span data-ttu-id="6c84d-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-144">publicador</span><span class="sxs-lookup"><span data-stu-id="6c84d-144">publisher</span></span>|<span data-ttu-id="6c84d-145">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-145">String</span></span>|<span data-ttu-id="6c84d-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-146">The publisher of the app.</span></span> <span data-ttu-id="6c84d-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6c84d-148">largeIcon</span></span>|[<span data-ttu-id="6c84d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6c84d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6c84d-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6c84d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6c84d-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c84d-152">createdDateTime</span></span>|<span data-ttu-id="6c84d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c84d-153">DateTimeOffset</span></span>|<span data-ttu-id="6c84d-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-154">The date and time the app was created.</span></span> <span data-ttu-id="6c84d-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c84d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6c84d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c84d-157">DateTimeOffset</span></span>|<span data-ttu-id="6c84d-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6c84d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6c84d-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6c84d-160">isFeatured</span></span>|<span data-ttu-id="6c84d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c84d-161">Boolean</span></span>|<span data-ttu-id="6c84d-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6c84d-163">privacyInformationUrl</span></span>|<span data-ttu-id="6c84d-164">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-164">String</span></span>|<span data-ttu-id="6c84d-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6c84d-165">The privacy statement Url.</span></span> <span data-ttu-id="6c84d-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6c84d-167">informationUrl</span></span>|<span data-ttu-id="6c84d-168">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-168">String</span></span>|<span data-ttu-id="6c84d-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6c84d-169">The more information Url.</span></span> <span data-ttu-id="6c84d-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-171">owner</span><span class="sxs-lookup"><span data-stu-id="6c84d-171">owner</span></span>|<span data-ttu-id="6c84d-172">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-172">String</span></span>|<span data-ttu-id="6c84d-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-173">The owner of the app.</span></span> <span data-ttu-id="6c84d-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-175">developer</span><span class="sxs-lookup"><span data-stu-id="6c84d-175">developer</span></span>|<span data-ttu-id="6c84d-176">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-176">String</span></span>|<span data-ttu-id="6c84d-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-177">The developer of the app.</span></span> <span data-ttu-id="6c84d-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-179">notes</span><span class="sxs-lookup"><span data-stu-id="6c84d-179">notes</span></span>|<span data-ttu-id="6c84d-180">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-180">String</span></span>|<span data-ttu-id="6c84d-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-181">Notes for the app.</span></span> <span data-ttu-id="6c84d-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6c84d-183">uploadState</span></span>|<span data-ttu-id="6c84d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6c84d-184">Int32</span></span>|<span data-ttu-id="6c84d-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="6c84d-185">The upload state.</span></span> <span data-ttu-id="6c84d-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6c84d-187">publishingState</span></span>|[<span data-ttu-id="6c84d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6c84d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6c84d-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-189">The publishing state for the app.</span></span> <span data-ttu-id="6c84d-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6c84d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6c84d-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c84d-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="6c84d-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6c84d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6c84d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6c84d-193">isAssigned</span></span>|<span data-ttu-id="6c84d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c84d-194">Boolean</span></span>|<span data-ttu-id="6c84d-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6c84d-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c84d-197">roleScopeTagIds</span></span>|<span data-ttu-id="6c84d-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c84d-198">String collection</span></span>|<span data-ttu-id="6c84d-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6c84d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6c84d-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6c84d-201">dependentAppCount</span></span>|<span data-ttu-id="6c84d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6c84d-202">Int32</span></span>|<span data-ttu-id="6c84d-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="6c84d-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6c84d-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="6c84d-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6c84d-205">appAvailability</span></span>|[<span data-ttu-id="6c84d-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="6c84d-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6c84d-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-207">The Application's availability.</span></span> <span data-ttu-id="6c84d-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6c84d-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6c84d-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6c84d-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6c84d-210">version</span><span class="sxs-lookup"><span data-stu-id="6c84d-210">version</span></span>|<span data-ttu-id="6c84d-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c84d-211">String</span></span>|<span data-ttu-id="6c84d-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c84d-212">The Application's version.</span></span> <span data-ttu-id="6c84d-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6c84d-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6c84d-214">committedContentVersion</span></span>|<span data-ttu-id="6c84d-215">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-215">String</span></span>|<span data-ttu-id="6c84d-216">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6c84d-216">The internal committed content version.</span></span> <span data-ttu-id="6c84d-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6c84d-218">fileName</span><span class="sxs-lookup"><span data-stu-id="6c84d-218">fileName</span></span>|<span data-ttu-id="6c84d-219">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-219">String</span></span>|<span data-ttu-id="6c84d-220">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6c84d-220">The name of the main Lob application file.</span></span> <span data-ttu-id="6c84d-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6c84d-222">size</span><span class="sxs-lookup"><span data-stu-id="6c84d-222">size</span></span>|<span data-ttu-id="6c84d-223">Int64</span><span class="sxs-lookup"><span data-stu-id="6c84d-223">Int64</span></span>|<span data-ttu-id="6c84d-224">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6c84d-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="6c84d-225">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6c84d-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6c84d-226">packageId</span><span class="sxs-lookup"><span data-stu-id="6c84d-226">packageId</span></span>|<span data-ttu-id="6c84d-227">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-227">String</span></span>|<span data-ttu-id="6c84d-228">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="6c84d-228">The package identifier.</span></span>|
|<span data-ttu-id="6c84d-229">identityName</span><span class="sxs-lookup"><span data-stu-id="6c84d-229">identityName</span></span>|<span data-ttu-id="6c84d-230">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-230">String</span></span>|<span data-ttu-id="6c84d-231">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6c84d-231">The Identity Name.</span></span>|
|<span data-ttu-id="6c84d-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6c84d-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6c84d-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6c84d-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="6c84d-234">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6c84d-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6c84d-235">versionName</span><span class="sxs-lookup"><span data-stu-id="6c84d-235">versionName</span></span>|<span data-ttu-id="6c84d-236">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-236">String</span></span>|<span data-ttu-id="6c84d-237">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6c84d-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6c84d-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="6c84d-238">versionCode</span></span>|<span data-ttu-id="6c84d-239">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-239">String</span></span>|<span data-ttu-id="6c84d-240">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6c84d-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6c84d-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6c84d-241">identityVersion</span></span>|<span data-ttu-id="6c84d-242">String</span><span class="sxs-lookup"><span data-stu-id="6c84d-242">String</span></span>|<span data-ttu-id="6c84d-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="6c84d-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="6c84d-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c84d-244">Response</span></span>
<span data-ttu-id="6c84d-245">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c84d-245">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c84d-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c84d-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c84d-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c84d-247">Request</span></span>
<span data-ttu-id="6c84d-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c84d-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1491

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="6c84d-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c84d-249">Response</span></span>
<span data-ttu-id="6c84d-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c84d-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1663

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




