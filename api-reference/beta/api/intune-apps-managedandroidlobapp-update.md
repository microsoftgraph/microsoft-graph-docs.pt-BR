---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 370273eb37e2095334b7ae4bbc25aded4a305545
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996147"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="80f25-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="80f25-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="80f25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80f25-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80f25-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80f25-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80f25-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80f25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80f25-107">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80f25-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80f25-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80f25-108">Prerequisites</span></span>
<span data-ttu-id="80f25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80f25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80f25-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80f25-111">Permission type</span></span>|<span data-ttu-id="80f25-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80f25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80f25-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80f25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80f25-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f25-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80f25-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80f25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80f25-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80f25-116">Not supported.</span></span>|
|<span data-ttu-id="80f25-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80f25-117">Application</span></span>|<span data-ttu-id="80f25-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f25-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80f25-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80f25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="80f25-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80f25-120">Request headers</span></span>
|<span data-ttu-id="80f25-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80f25-121">Header</span></span>|<span data-ttu-id="80f25-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80f25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80f25-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80f25-123">Authorization</span></span>|<span data-ttu-id="80f25-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80f25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80f25-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80f25-125">Accept</span></span>|<span data-ttu-id="80f25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80f25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80f25-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80f25-127">Request body</span></span>
<span data-ttu-id="80f25-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80f25-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="80f25-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="80f25-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="80f25-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80f25-130">Property</span></span>|<span data-ttu-id="80f25-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80f25-131">Type</span></span>|<span data-ttu-id="80f25-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80f25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f25-133">id</span><span class="sxs-lookup"><span data-stu-id="80f25-133">id</span></span>|<span data-ttu-id="80f25-134">String</span><span class="sxs-lookup"><span data-stu-id="80f25-134">String</span></span>|<span data-ttu-id="80f25-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80f25-135">Key of the entity.</span></span> <span data-ttu-id="80f25-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-137">displayName</span><span class="sxs-lookup"><span data-stu-id="80f25-137">displayName</span></span>|<span data-ttu-id="80f25-138">String</span><span class="sxs-lookup"><span data-stu-id="80f25-138">String</span></span>|<span data-ttu-id="80f25-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="80f25-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80f25-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-141">description</span><span class="sxs-lookup"><span data-stu-id="80f25-141">description</span></span>|<span data-ttu-id="80f25-142">String</span><span class="sxs-lookup"><span data-stu-id="80f25-142">String</span></span>|<span data-ttu-id="80f25-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-143">The description of the app.</span></span> <span data-ttu-id="80f25-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-145">publicador</span><span class="sxs-lookup"><span data-stu-id="80f25-145">publisher</span></span>|<span data-ttu-id="80f25-146">String</span><span class="sxs-lookup"><span data-stu-id="80f25-146">String</span></span>|<span data-ttu-id="80f25-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-147">The publisher of the app.</span></span> <span data-ttu-id="80f25-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80f25-149">largeIcon</span></span>|[<span data-ttu-id="80f25-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80f25-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="80f25-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="80f25-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80f25-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80f25-153">createdDateTime</span></span>|<span data-ttu-id="80f25-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f25-154">DateTimeOffset</span></span>|<span data-ttu-id="80f25-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-155">The date and time the app was created.</span></span> <span data-ttu-id="80f25-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80f25-157">lastModifiedDateTime</span></span>|<span data-ttu-id="80f25-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80f25-158">DateTimeOffset</span></span>|<span data-ttu-id="80f25-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="80f25-159">The date and time the app was last modified.</span></span> <span data-ttu-id="80f25-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80f25-161">isFeatured</span></span>|<span data-ttu-id="80f25-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f25-162">Boolean</span></span>|<span data-ttu-id="80f25-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80f25-164">privacyInformationUrl</span></span>|<span data-ttu-id="80f25-165">String</span><span class="sxs-lookup"><span data-stu-id="80f25-165">String</span></span>|<span data-ttu-id="80f25-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="80f25-166">The privacy statement Url.</span></span> <span data-ttu-id="80f25-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80f25-168">informationUrl</span></span>|<span data-ttu-id="80f25-169">String</span><span class="sxs-lookup"><span data-stu-id="80f25-169">String</span></span>|<span data-ttu-id="80f25-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="80f25-170">The more information Url.</span></span> <span data-ttu-id="80f25-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-172">proprietário</span><span class="sxs-lookup"><span data-stu-id="80f25-172">owner</span></span>|<span data-ttu-id="80f25-173">String</span><span class="sxs-lookup"><span data-stu-id="80f25-173">String</span></span>|<span data-ttu-id="80f25-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="80f25-174">The owner of the app.</span></span> <span data-ttu-id="80f25-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-176">developer</span><span class="sxs-lookup"><span data-stu-id="80f25-176">developer</span></span>|<span data-ttu-id="80f25-177">String</span><span class="sxs-lookup"><span data-stu-id="80f25-177">String</span></span>|<span data-ttu-id="80f25-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-178">The developer of the app.</span></span> <span data-ttu-id="80f25-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-180">notes</span><span class="sxs-lookup"><span data-stu-id="80f25-180">notes</span></span>|<span data-ttu-id="80f25-181">String</span><span class="sxs-lookup"><span data-stu-id="80f25-181">String</span></span>|<span data-ttu-id="80f25-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-182">Notes for the app.</span></span> <span data-ttu-id="80f25-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="80f25-184">uploadState</span></span>|<span data-ttu-id="80f25-185">Int32</span><span class="sxs-lookup"><span data-stu-id="80f25-185">Int32</span></span>|<span data-ttu-id="80f25-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="80f25-186">The upload state.</span></span> <span data-ttu-id="80f25-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="80f25-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="80f25-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="80f25-189">publishingState</span></span>|[<span data-ttu-id="80f25-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80f25-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="80f25-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-191">The publishing state for the app.</span></span> <span data-ttu-id="80f25-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="80f25-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80f25-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="80f25-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="80f25-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="80f25-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80f25-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="80f25-195">isAssigned</span></span>|<span data-ttu-id="80f25-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="80f25-196">Boolean</span></span>|<span data-ttu-id="80f25-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="80f25-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="80f25-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80f25-199">roleScopeTagIds</span></span>|<span data-ttu-id="80f25-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="80f25-200">String collection</span></span>|<span data-ttu-id="80f25-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="80f25-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="80f25-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="80f25-203">dependentAppCount</span></span>|<span data-ttu-id="80f25-204">Int32</span><span class="sxs-lookup"><span data-stu-id="80f25-204">Int32</span></span>|<span data-ttu-id="80f25-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="80f25-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="80f25-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="80f25-207">supersedingAppCount</span></span>|<span data-ttu-id="80f25-208">Int32</span><span class="sxs-lookup"><span data-stu-id="80f25-208">Int32</span></span>|<span data-ttu-id="80f25-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="80f25-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="80f25-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="80f25-211">supersededAppCount</span></span>|<span data-ttu-id="80f25-212">Int32</span><span class="sxs-lookup"><span data-stu-id="80f25-212">Int32</span></span>|<span data-ttu-id="80f25-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="80f25-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="80f25-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="80f25-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="80f25-215">appAvailability</span></span>|[<span data-ttu-id="80f25-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="80f25-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="80f25-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-217">The Application's availability.</span></span> <span data-ttu-id="80f25-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="80f25-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="80f25-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="80f25-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="80f25-220">version</span><span class="sxs-lookup"><span data-stu-id="80f25-220">version</span></span>|<span data-ttu-id="80f25-221">String</span><span class="sxs-lookup"><span data-stu-id="80f25-221">String</span></span>|<span data-ttu-id="80f25-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80f25-222">The Application's version.</span></span> <span data-ttu-id="80f25-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="80f25-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="80f25-224">committedContentVersion</span></span>|<span data-ttu-id="80f25-225">String</span><span class="sxs-lookup"><span data-stu-id="80f25-225">String</span></span>|<span data-ttu-id="80f25-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="80f25-226">The internal committed content version.</span></span> <span data-ttu-id="80f25-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="80f25-228">fileName</span><span class="sxs-lookup"><span data-stu-id="80f25-228">fileName</span></span>|<span data-ttu-id="80f25-229">String</span><span class="sxs-lookup"><span data-stu-id="80f25-229">String</span></span>|<span data-ttu-id="80f25-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="80f25-230">The name of the main Lob application file.</span></span> <span data-ttu-id="80f25-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="80f25-232">size</span><span class="sxs-lookup"><span data-stu-id="80f25-232">size</span></span>|<span data-ttu-id="80f25-233">Int64</span><span class="sxs-lookup"><span data-stu-id="80f25-233">Int64</span></span>|<span data-ttu-id="80f25-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="80f25-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="80f25-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="80f25-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="80f25-236">packageId</span><span class="sxs-lookup"><span data-stu-id="80f25-236">packageId</span></span>|<span data-ttu-id="80f25-237">String</span><span class="sxs-lookup"><span data-stu-id="80f25-237">String</span></span>|<span data-ttu-id="80f25-238">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="80f25-238">The package identifier.</span></span>|
|<span data-ttu-id="80f25-239">identityName</span><span class="sxs-lookup"><span data-stu-id="80f25-239">identityName</span></span>|<span data-ttu-id="80f25-240">String</span><span class="sxs-lookup"><span data-stu-id="80f25-240">String</span></span>|<span data-ttu-id="80f25-241">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="80f25-241">The Identity Name.</span></span>|
|<span data-ttu-id="80f25-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80f25-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="80f25-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="80f25-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="80f25-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="80f25-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="80f25-245">versionName</span><span class="sxs-lookup"><span data-stu-id="80f25-245">versionName</span></span>|<span data-ttu-id="80f25-246">String</span><span class="sxs-lookup"><span data-stu-id="80f25-246">String</span></span>|<span data-ttu-id="80f25-247">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="80f25-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="80f25-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="80f25-248">versionCode</span></span>|<span data-ttu-id="80f25-249">String</span><span class="sxs-lookup"><span data-stu-id="80f25-249">String</span></span>|<span data-ttu-id="80f25-250">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="80f25-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="80f25-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="80f25-251">identityVersion</span></span>|<span data-ttu-id="80f25-252">String</span><span class="sxs-lookup"><span data-stu-id="80f25-252">String</span></span>|<span data-ttu-id="80f25-253">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="80f25-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="80f25-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="80f25-254">Response</span></span>
<span data-ttu-id="80f25-255">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80f25-255">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f25-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80f25-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="80f25-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80f25-257">Request</span></span>
<span data-ttu-id="80f25-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80f25-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1548

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="80f25-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="80f25-259">Response</span></span>
<span data-ttu-id="80f25-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80f25-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1720

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
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```






