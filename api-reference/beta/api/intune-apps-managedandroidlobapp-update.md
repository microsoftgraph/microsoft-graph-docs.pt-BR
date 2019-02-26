---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e43a6b1babb23c56818391e6fd89da58005dd8e0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157502"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="e13ba-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e13ba-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="e13ba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e13ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e13ba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e13ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e13ba-106">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-106">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e13ba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e13ba-107">Prerequisites</span></span>
<span data-ttu-id="e13ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e13ba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e13ba-110">Permission type</span></span>|<span data-ttu-id="e13ba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e13ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e13ba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e13ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e13ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e13ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e13ba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e13ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e13ba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13ba-115">Not supported.</span></span>|
|<span data-ttu-id="e13ba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e13ba-116">Application</span></span>|<span data-ttu-id="e13ba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e13ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e13ba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e13ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e13ba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e13ba-119">Request headers</span></span>
|<span data-ttu-id="e13ba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e13ba-120">Header</span></span>|<span data-ttu-id="e13ba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e13ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e13ba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e13ba-122">Authorization</span></span>|<span data-ttu-id="e13ba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e13ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e13ba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e13ba-124">Accept</span></span>|<span data-ttu-id="e13ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e13ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e13ba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e13ba-126">Request body</span></span>
<span data-ttu-id="e13ba-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-127">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="e13ba-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-128">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="e13ba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e13ba-129">Property</span></span>|<span data-ttu-id="e13ba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e13ba-130">Type</span></span>|<span data-ttu-id="e13ba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e13ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e13ba-132">id</span><span class="sxs-lookup"><span data-stu-id="e13ba-132">id</span></span>|<span data-ttu-id="e13ba-133">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-133">String</span></span>|<span data-ttu-id="e13ba-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e13ba-134">Key of the entity.</span></span> <span data-ttu-id="e13ba-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e13ba-136">displayName</span></span>|<span data-ttu-id="e13ba-137">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-137">String</span></span>|<span data-ttu-id="e13ba-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e13ba-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e13ba-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-140">description</span><span class="sxs-lookup"><span data-stu-id="e13ba-140">description</span></span>|<span data-ttu-id="e13ba-141">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-141">String</span></span>|<span data-ttu-id="e13ba-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-142">The description of the app.</span></span> <span data-ttu-id="e13ba-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e13ba-144">publisher</span></span>|<span data-ttu-id="e13ba-145">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-145">String</span></span>|<span data-ttu-id="e13ba-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-146">The publisher of the app.</span></span> <span data-ttu-id="e13ba-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e13ba-148">largeIcon</span></span>|[<span data-ttu-id="e13ba-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e13ba-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e13ba-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e13ba-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e13ba-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e13ba-152">createdDateTime</span></span>|<span data-ttu-id="e13ba-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e13ba-153">DateTimeOffset</span></span>|<span data-ttu-id="e13ba-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-154">The date and time the app was created.</span></span> <span data-ttu-id="e13ba-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e13ba-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e13ba-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e13ba-157">DateTimeOffset</span></span>|<span data-ttu-id="e13ba-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e13ba-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e13ba-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e13ba-160">isFeatured</span></span>|<span data-ttu-id="e13ba-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e13ba-161">Boolean</span></span>|<span data-ttu-id="e13ba-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e13ba-163">privacyInformationUrl</span></span>|<span data-ttu-id="e13ba-164">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-164">String</span></span>|<span data-ttu-id="e13ba-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e13ba-165">The privacy statement Url.</span></span> <span data-ttu-id="e13ba-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e13ba-167">informationUrl</span></span>|<span data-ttu-id="e13ba-168">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-168">String</span></span>|<span data-ttu-id="e13ba-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e13ba-169">The more information Url.</span></span> <span data-ttu-id="e13ba-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-171">owner</span><span class="sxs-lookup"><span data-stu-id="e13ba-171">owner</span></span>|<span data-ttu-id="e13ba-172">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-172">String</span></span>|<span data-ttu-id="e13ba-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-173">The owner of the app.</span></span> <span data-ttu-id="e13ba-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-175">developer</span><span class="sxs-lookup"><span data-stu-id="e13ba-175">developer</span></span>|<span data-ttu-id="e13ba-176">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-176">String</span></span>|<span data-ttu-id="e13ba-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-177">The developer of the app.</span></span> <span data-ttu-id="e13ba-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-179">Observações</span><span class="sxs-lookup"><span data-stu-id="e13ba-179">notes</span></span>|<span data-ttu-id="e13ba-180">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-180">String</span></span>|<span data-ttu-id="e13ba-181">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-181">Notes for the app.</span></span> <span data-ttu-id="e13ba-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e13ba-183">uploadState</span></span>|<span data-ttu-id="e13ba-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e13ba-184">Int32</span></span>|<span data-ttu-id="e13ba-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e13ba-185">The upload state.</span></span> <span data-ttu-id="e13ba-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e13ba-187">publishingState</span></span>|[<span data-ttu-id="e13ba-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e13ba-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e13ba-189">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-189">The publishing state for the app.</span></span> <span data-ttu-id="e13ba-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e13ba-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e13ba-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e13ba-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e13ba-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e13ba-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e13ba-193">isAssigned</span></span>|<span data-ttu-id="e13ba-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e13ba-194">Boolean</span></span>|<span data-ttu-id="e13ba-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e13ba-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e13ba-197">roleScopeTagIds</span></span>|<span data-ttu-id="e13ba-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e13ba-198">String collection</span></span>|<span data-ttu-id="e13ba-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e13ba-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e13ba-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e13ba-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e13ba-201">appAvailability</span></span>|[<span data-ttu-id="e13ba-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e13ba-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e13ba-203">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-203">The Application's availability.</span></span> <span data-ttu-id="e13ba-204">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="e13ba-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e13ba-205">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="e13ba-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e13ba-206">version</span><span class="sxs-lookup"><span data-stu-id="e13ba-206">version</span></span>|<span data-ttu-id="e13ba-207">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-207">String</span></span>|<span data-ttu-id="e13ba-208">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e13ba-208">The Application's version.</span></span> <span data-ttu-id="e13ba-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e13ba-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e13ba-210">committedContentVersion</span></span>|<span data-ttu-id="e13ba-211">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-211">String</span></span>|<span data-ttu-id="e13ba-212">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="e13ba-212">The internal committed content version.</span></span> <span data-ttu-id="e13ba-213">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e13ba-214">fileName</span><span class="sxs-lookup"><span data-stu-id="e13ba-214">fileName</span></span>|<span data-ttu-id="e13ba-215">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-215">String</span></span>|<span data-ttu-id="e13ba-216">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="e13ba-216">The name of the main Lob application file.</span></span> <span data-ttu-id="e13ba-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e13ba-218">size</span><span class="sxs-lookup"><span data-stu-id="e13ba-218">size</span></span>|<span data-ttu-id="e13ba-219">Int64</span><span class="sxs-lookup"><span data-stu-id="e13ba-219">Int64</span></span>|<span data-ttu-id="e13ba-220">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="e13ba-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="e13ba-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e13ba-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e13ba-222">packageId</span><span class="sxs-lookup"><span data-stu-id="e13ba-222">packageId</span></span>|<span data-ttu-id="e13ba-223">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-223">String</span></span>|<span data-ttu-id="e13ba-224">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="e13ba-224">The package identifier.</span></span>|
|<span data-ttu-id="e13ba-225">identityName</span><span class="sxs-lookup"><span data-stu-id="e13ba-225">identityName</span></span>|<span data-ttu-id="e13ba-226">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-226">String</span></span>|<span data-ttu-id="e13ba-227">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e13ba-227">The Identity Name.</span></span>|
|<span data-ttu-id="e13ba-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e13ba-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e13ba-229">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e13ba-229">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e13ba-230">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e13ba-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e13ba-231">versionName</span><span class="sxs-lookup"><span data-stu-id="e13ba-231">versionName</span></span>|<span data-ttu-id="e13ba-232">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-232">String</span></span>|<span data-ttu-id="e13ba-233">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e13ba-233">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e13ba-234">versionCode</span><span class="sxs-lookup"><span data-stu-id="e13ba-234">versionCode</span></span>|<span data-ttu-id="e13ba-235">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-235">String</span></span>|<span data-ttu-id="e13ba-236">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e13ba-236">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e13ba-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e13ba-237">identityVersion</span></span>|<span data-ttu-id="e13ba-238">String</span><span class="sxs-lookup"><span data-stu-id="e13ba-238">String</span></span>|<span data-ttu-id="e13ba-239">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="e13ba-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e13ba-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13ba-240">Response</span></span>
<span data-ttu-id="e13ba-241">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e13ba-241">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e13ba-242">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e13ba-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="e13ba-243">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e13ba-243">Request</span></span>
<span data-ttu-id="e13ba-244">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e13ba-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1464

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

### <a name="response"></a><span data-ttu-id="e13ba-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="e13ba-245">Response</span></span>
<span data-ttu-id="e13ba-p123">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e13ba-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1636

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




