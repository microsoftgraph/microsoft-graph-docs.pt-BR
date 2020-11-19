---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5eb4c62c6f3b61550e93c08e4674ba07d79da87d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49250734"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="bcbef-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="bcbef-103">Update managedAndroidLobApp</span></span>

<span data-ttu-id="bcbef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcbef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bcbef-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bcbef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bcbef-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bcbef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bcbef-107">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcbef-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bcbef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bcbef-108">Prerequisites</span></span>
<span data-ttu-id="bcbef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcbef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcbef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bcbef-111">Permission type</span></span>|<span data-ttu-id="bcbef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bcbef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcbef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bcbef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcbef-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbef-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bcbef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bcbef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcbef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bcbef-116">Not supported.</span></span>|
|<span data-ttu-id="bcbef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bcbef-117">Application</span></span>|<span data-ttu-id="bcbef-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcbef-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcbef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bcbef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bcbef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbef-120">Request headers</span></span>
|<span data-ttu-id="bcbef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bcbef-121">Header</span></span>|<span data-ttu-id="bcbef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bcbef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcbef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bcbef-123">Authorization</span></span>|<span data-ttu-id="bcbef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bcbef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcbef-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bcbef-125">Accept</span></span>|<span data-ttu-id="bcbef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bcbef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcbef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbef-127">Request body</span></span>
<span data-ttu-id="bcbef-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcbef-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="bcbef-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcbef-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="bcbef-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bcbef-130">Property</span></span>|<span data-ttu-id="bcbef-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bcbef-131">Type</span></span>|<span data-ttu-id="bcbef-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bcbef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bcbef-133">id</span><span class="sxs-lookup"><span data-stu-id="bcbef-133">id</span></span>|<span data-ttu-id="bcbef-134">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-134">String</span></span>|<span data-ttu-id="bcbef-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bcbef-135">Key of the entity.</span></span> <span data-ttu-id="bcbef-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bcbef-137">displayName</span></span>|<span data-ttu-id="bcbef-138">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-138">String</span></span>|<span data-ttu-id="bcbef-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bcbef-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bcbef-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-141">description</span><span class="sxs-lookup"><span data-stu-id="bcbef-141">description</span></span>|<span data-ttu-id="bcbef-142">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-142">String</span></span>|<span data-ttu-id="bcbef-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-143">The description of the app.</span></span> <span data-ttu-id="bcbef-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-145">publicador</span><span class="sxs-lookup"><span data-stu-id="bcbef-145">publisher</span></span>|<span data-ttu-id="bcbef-146">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-146">String</span></span>|<span data-ttu-id="bcbef-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-147">The publisher of the app.</span></span> <span data-ttu-id="bcbef-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bcbef-149">largeIcon</span></span>|[<span data-ttu-id="bcbef-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bcbef-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bcbef-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bcbef-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bcbef-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bcbef-153">createdDateTime</span></span>|<span data-ttu-id="bcbef-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcbef-154">DateTimeOffset</span></span>|<span data-ttu-id="bcbef-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-155">The date and time the app was created.</span></span> <span data-ttu-id="bcbef-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bcbef-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bcbef-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bcbef-158">DateTimeOffset</span></span>|<span data-ttu-id="bcbef-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bcbef-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bcbef-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bcbef-161">isFeatured</span></span>|<span data-ttu-id="bcbef-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcbef-162">Boolean</span></span>|<span data-ttu-id="bcbef-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bcbef-164">privacyInformationUrl</span></span>|<span data-ttu-id="bcbef-165">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-165">String</span></span>|<span data-ttu-id="bcbef-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bcbef-166">The privacy statement Url.</span></span> <span data-ttu-id="bcbef-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bcbef-168">informationUrl</span></span>|<span data-ttu-id="bcbef-169">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-169">String</span></span>|<span data-ttu-id="bcbef-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bcbef-170">The more information Url.</span></span> <span data-ttu-id="bcbef-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-172">owner</span><span class="sxs-lookup"><span data-stu-id="bcbef-172">owner</span></span>|<span data-ttu-id="bcbef-173">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-173">String</span></span>|<span data-ttu-id="bcbef-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-174">The owner of the app.</span></span> <span data-ttu-id="bcbef-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-176">developer</span><span class="sxs-lookup"><span data-stu-id="bcbef-176">developer</span></span>|<span data-ttu-id="bcbef-177">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-177">String</span></span>|<span data-ttu-id="bcbef-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-178">The developer of the app.</span></span> <span data-ttu-id="bcbef-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-180">notes</span><span class="sxs-lookup"><span data-stu-id="bcbef-180">notes</span></span>|<span data-ttu-id="bcbef-181">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-181">String</span></span>|<span data-ttu-id="bcbef-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-182">Notes for the app.</span></span> <span data-ttu-id="bcbef-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bcbef-184">uploadState</span></span>|<span data-ttu-id="bcbef-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbef-185">Int32</span></span>|<span data-ttu-id="bcbef-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="bcbef-186">The upload state.</span></span> <span data-ttu-id="bcbef-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="bcbef-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bcbef-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bcbef-189">publishingState</span></span>|[<span data-ttu-id="bcbef-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bcbef-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bcbef-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-191">The publishing state for the app.</span></span> <span data-ttu-id="bcbef-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bcbef-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bcbef-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcbef-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bcbef-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bcbef-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bcbef-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bcbef-195">isAssigned</span></span>|<span data-ttu-id="bcbef-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bcbef-196">Boolean</span></span>|<span data-ttu-id="bcbef-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bcbef-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bcbef-199">roleScopeTagIds</span></span>|<span data-ttu-id="bcbef-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bcbef-200">String collection</span></span>|<span data-ttu-id="bcbef-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bcbef-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bcbef-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bcbef-203">dependentAppCount</span></span>|<span data-ttu-id="bcbef-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbef-204">Int32</span></span>|<span data-ttu-id="bcbef-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="bcbef-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bcbef-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="bcbef-207">supersedingAppCount</span></span>|<span data-ttu-id="bcbef-208">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbef-208">Int32</span></span>|<span data-ttu-id="bcbef-209">O número total de aplicativos que este aplicativo substitui direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="bcbef-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="bcbef-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="bcbef-211">supersededAppCount</span></span>|<span data-ttu-id="bcbef-212">Int32</span><span class="sxs-lookup"><span data-stu-id="bcbef-212">Int32</span></span>|<span data-ttu-id="bcbef-213">O número total de aplicativos que este aplicativo está substituindo direta ou indiretamente por.</span><span class="sxs-lookup"><span data-stu-id="bcbef-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="bcbef-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bcbef-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bcbef-215">appAvailability</span></span>|[<span data-ttu-id="bcbef-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bcbef-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bcbef-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-217">The Application's availability.</span></span> <span data-ttu-id="bcbef-218">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bcbef-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bcbef-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bcbef-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bcbef-220">version</span><span class="sxs-lookup"><span data-stu-id="bcbef-220">version</span></span>|<span data-ttu-id="bcbef-221">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-221">String</span></span>|<span data-ttu-id="bcbef-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bcbef-222">The Application's version.</span></span> <span data-ttu-id="bcbef-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bcbef-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bcbef-224">committedContentVersion</span></span>|<span data-ttu-id="bcbef-225">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-225">String</span></span>|<span data-ttu-id="bcbef-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="bcbef-226">The internal committed content version.</span></span> <span data-ttu-id="bcbef-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bcbef-228">fileName</span><span class="sxs-lookup"><span data-stu-id="bcbef-228">fileName</span></span>|<span data-ttu-id="bcbef-229">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-229">String</span></span>|<span data-ttu-id="bcbef-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="bcbef-230">The name of the main Lob application file.</span></span> <span data-ttu-id="bcbef-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bcbef-232">size</span><span class="sxs-lookup"><span data-stu-id="bcbef-232">size</span></span>|<span data-ttu-id="bcbef-233">Int64</span><span class="sxs-lookup"><span data-stu-id="bcbef-233">Int64</span></span>|<span data-ttu-id="bcbef-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="bcbef-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="bcbef-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bcbef-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bcbef-236">packageId</span><span class="sxs-lookup"><span data-stu-id="bcbef-236">packageId</span></span>|<span data-ttu-id="bcbef-237">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-237">String</span></span>|<span data-ttu-id="bcbef-238">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="bcbef-238">The package identifier.</span></span>|
|<span data-ttu-id="bcbef-239">identityName</span><span class="sxs-lookup"><span data-stu-id="bcbef-239">identityName</span></span>|<span data-ttu-id="bcbef-240">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-240">String</span></span>|<span data-ttu-id="bcbef-241">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="bcbef-241">The Identity Name.</span></span>|
|<span data-ttu-id="bcbef-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bcbef-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bcbef-243">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bcbef-243">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="bcbef-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="bcbef-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bcbef-245">versionName</span><span class="sxs-lookup"><span data-stu-id="bcbef-245">versionName</span></span>|<span data-ttu-id="bcbef-246">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-246">String</span></span>|<span data-ttu-id="bcbef-247">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bcbef-247">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bcbef-248">versionCode</span><span class="sxs-lookup"><span data-stu-id="bcbef-248">versionCode</span></span>|<span data-ttu-id="bcbef-249">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-249">String</span></span>|<span data-ttu-id="bcbef-250">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bcbef-250">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bcbef-251">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bcbef-251">identityVersion</span></span>|<span data-ttu-id="bcbef-252">String</span><span class="sxs-lookup"><span data-stu-id="bcbef-252">String</span></span>|<span data-ttu-id="bcbef-253">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="bcbef-253">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="bcbef-254">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbef-254">Response</span></span>
<span data-ttu-id="bcbef-255">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bcbef-255">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcbef-256">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bcbef-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="bcbef-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bcbef-257">Request</span></span>
<span data-ttu-id="bcbef-258">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bcbef-258">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bcbef-259">Resposta</span><span class="sxs-lookup"><span data-stu-id="bcbef-259">Response</span></span>
<span data-ttu-id="bcbef-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bcbef-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




