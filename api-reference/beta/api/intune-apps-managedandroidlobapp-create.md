---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87dd096b5da77b55248c7e896721022b6b0f83ac
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791992"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="ea789-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="ea789-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="ea789-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea789-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea789-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea789-107">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="ea789-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ea789-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ea789-108">Prerequisites</span></span>
<span data-ttu-id="ea789-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea789-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea789-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea789-111">Permission type</span></span>|<span data-ttu-id="ea789-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ea789-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea789-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea789-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea789-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea789-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea789-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea789-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea789-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea789-116">Not supported.</span></span>|
|<span data-ttu-id="ea789-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea789-117">Application</span></span>|<span data-ttu-id="ea789-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea789-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea789-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea789-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ea789-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea789-120">Request headers</span></span>
|<span data-ttu-id="ea789-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ea789-121">Header</span></span>|<span data-ttu-id="ea789-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ea789-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea789-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea789-123">Authorization</span></span>|<span data-ttu-id="ea789-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea789-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea789-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ea789-125">Accept</span></span>|<span data-ttu-id="ea789-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea789-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea789-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea789-127">Request body</span></span>
<span data-ttu-id="ea789-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="ea789-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="ea789-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="ea789-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="ea789-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea789-130">Property</span></span>|<span data-ttu-id="ea789-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea789-131">Type</span></span>|<span data-ttu-id="ea789-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea789-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea789-133">id</span><span class="sxs-lookup"><span data-stu-id="ea789-133">id</span></span>|<span data-ttu-id="ea789-134">String</span><span class="sxs-lookup"><span data-stu-id="ea789-134">String</span></span>|<span data-ttu-id="ea789-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea789-135">Key of the entity.</span></span> <span data-ttu-id="ea789-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ea789-137">displayName</span></span>|<span data-ttu-id="ea789-138">String</span><span class="sxs-lookup"><span data-stu-id="ea789-138">String</span></span>|<span data-ttu-id="ea789-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ea789-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ea789-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-141">description</span><span class="sxs-lookup"><span data-stu-id="ea789-141">description</span></span>|<span data-ttu-id="ea789-142">String</span><span class="sxs-lookup"><span data-stu-id="ea789-142">String</span></span>|<span data-ttu-id="ea789-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-143">The description of the app.</span></span> <span data-ttu-id="ea789-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-145">publicador</span><span class="sxs-lookup"><span data-stu-id="ea789-145">publisher</span></span>|<span data-ttu-id="ea789-146">String</span><span class="sxs-lookup"><span data-stu-id="ea789-146">String</span></span>|<span data-ttu-id="ea789-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-147">The publisher of the app.</span></span> <span data-ttu-id="ea789-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ea789-149">largeIcon</span></span>|[<span data-ttu-id="ea789-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ea789-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ea789-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ea789-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ea789-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea789-153">createdDateTime</span></span>|<span data-ttu-id="ea789-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea789-154">DateTimeOffset</span></span>|<span data-ttu-id="ea789-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-155">The date and time the app was created.</span></span> <span data-ttu-id="ea789-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea789-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ea789-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea789-158">DateTimeOffset</span></span>|<span data-ttu-id="ea789-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ea789-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ea789-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ea789-161">isFeatured</span></span>|<span data-ttu-id="ea789-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea789-162">Boolean</span></span>|<span data-ttu-id="ea789-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ea789-164">privacyInformationUrl</span></span>|<span data-ttu-id="ea789-165">String</span><span class="sxs-lookup"><span data-stu-id="ea789-165">String</span></span>|<span data-ttu-id="ea789-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ea789-166">The privacy statement Url.</span></span> <span data-ttu-id="ea789-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ea789-168">informationUrl</span></span>|<span data-ttu-id="ea789-169">String</span><span class="sxs-lookup"><span data-stu-id="ea789-169">String</span></span>|<span data-ttu-id="ea789-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ea789-170">The more information Url.</span></span> <span data-ttu-id="ea789-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-172">owner</span><span class="sxs-lookup"><span data-stu-id="ea789-172">owner</span></span>|<span data-ttu-id="ea789-173">String</span><span class="sxs-lookup"><span data-stu-id="ea789-173">String</span></span>|<span data-ttu-id="ea789-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ea789-174">The owner of the app.</span></span> <span data-ttu-id="ea789-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-176">developer</span><span class="sxs-lookup"><span data-stu-id="ea789-176">developer</span></span>|<span data-ttu-id="ea789-177">String</span><span class="sxs-lookup"><span data-stu-id="ea789-177">String</span></span>|<span data-ttu-id="ea789-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-178">The developer of the app.</span></span> <span data-ttu-id="ea789-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-180">notes</span><span class="sxs-lookup"><span data-stu-id="ea789-180">notes</span></span>|<span data-ttu-id="ea789-181">String</span><span class="sxs-lookup"><span data-stu-id="ea789-181">String</span></span>|<span data-ttu-id="ea789-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-182">Notes for the app.</span></span> <span data-ttu-id="ea789-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ea789-184">uploadState</span></span>|<span data-ttu-id="ea789-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ea789-185">Int32</span></span>|<span data-ttu-id="ea789-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ea789-186">The upload state.</span></span> <span data-ttu-id="ea789-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="ea789-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ea789-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ea789-189">publishingState</span></span>|[<span data-ttu-id="ea789-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ea789-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ea789-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-191">The publishing state for the app.</span></span> <span data-ttu-id="ea789-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ea789-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ea789-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ea789-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ea789-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ea789-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ea789-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ea789-195">isAssigned</span></span>|<span data-ttu-id="ea789-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea789-196">Boolean</span></span>|<span data-ttu-id="ea789-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ea789-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ea789-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ea789-199">roleScopeTagIds</span></span>|<span data-ttu-id="ea789-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea789-200">String collection</span></span>|<span data-ttu-id="ea789-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ea789-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ea789-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ea789-203">dependentAppCount</span></span>|<span data-ttu-id="ea789-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ea789-204">Int32</span></span>|<span data-ttu-id="ea789-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ea789-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ea789-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ea789-207">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ea789-207">appAvailability</span></span>|[<span data-ttu-id="ea789-208">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ea789-208">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ea789-209">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-209">The Application's availability.</span></span> <span data-ttu-id="ea789-210">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ea789-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ea789-211">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="ea789-211">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ea789-212">version</span><span class="sxs-lookup"><span data-stu-id="ea789-212">version</span></span>|<span data-ttu-id="ea789-213">String</span><span class="sxs-lookup"><span data-stu-id="ea789-213">String</span></span>|<span data-ttu-id="ea789-214">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea789-214">The Application's version.</span></span> <span data-ttu-id="ea789-215">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-215">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ea789-216">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ea789-216">committedContentVersion</span></span>|<span data-ttu-id="ea789-217">String</span><span class="sxs-lookup"><span data-stu-id="ea789-217">String</span></span>|<span data-ttu-id="ea789-218">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="ea789-218">The internal committed content version.</span></span> <span data-ttu-id="ea789-219">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-219">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ea789-220">fileName</span><span class="sxs-lookup"><span data-stu-id="ea789-220">fileName</span></span>|<span data-ttu-id="ea789-221">String</span><span class="sxs-lookup"><span data-stu-id="ea789-221">String</span></span>|<span data-ttu-id="ea789-222">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="ea789-222">The name of the main Lob application file.</span></span> <span data-ttu-id="ea789-223">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-223">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ea789-224">size</span><span class="sxs-lookup"><span data-stu-id="ea789-224">size</span></span>|<span data-ttu-id="ea789-225">Int64</span><span class="sxs-lookup"><span data-stu-id="ea789-225">Int64</span></span>|<span data-ttu-id="ea789-226">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="ea789-226">The total size, including all uploaded files.</span></span> <span data-ttu-id="ea789-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea789-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ea789-228">packageId</span><span class="sxs-lookup"><span data-stu-id="ea789-228">packageId</span></span>|<span data-ttu-id="ea789-229">String</span><span class="sxs-lookup"><span data-stu-id="ea789-229">String</span></span>|<span data-ttu-id="ea789-230">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="ea789-230">The package identifier.</span></span>|
|<span data-ttu-id="ea789-231">identityName</span><span class="sxs-lookup"><span data-stu-id="ea789-231">identityName</span></span>|<span data-ttu-id="ea789-232">String</span><span class="sxs-lookup"><span data-stu-id="ea789-232">String</span></span>|<span data-ttu-id="ea789-233">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ea789-233">The Identity Name.</span></span>|
|<span data-ttu-id="ea789-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea789-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ea789-235">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea789-235">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ea789-236">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="ea789-236">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ea789-237">versionName</span><span class="sxs-lookup"><span data-stu-id="ea789-237">versionName</span></span>|<span data-ttu-id="ea789-238">String</span><span class="sxs-lookup"><span data-stu-id="ea789-238">String</span></span>|<span data-ttu-id="ea789-239">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ea789-239">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ea789-240">versionCode</span><span class="sxs-lookup"><span data-stu-id="ea789-240">versionCode</span></span>|<span data-ttu-id="ea789-241">String</span><span class="sxs-lookup"><span data-stu-id="ea789-241">String</span></span>|<span data-ttu-id="ea789-242">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="ea789-242">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ea789-243">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ea789-243">identityVersion</span></span>|<span data-ttu-id="ea789-244">String</span><span class="sxs-lookup"><span data-stu-id="ea789-244">String</span></span>|<span data-ttu-id="ea789-245">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="ea789-245">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ea789-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea789-246">Response</span></span>
<span data-ttu-id="ea789-247">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea789-247">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea789-248">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea789-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea789-249">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea789-249">Request</span></span>
<span data-ttu-id="ea789-250">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ea789-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="ea789-251">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea789-251">Response</span></span>
<span data-ttu-id="ea789-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea789-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



