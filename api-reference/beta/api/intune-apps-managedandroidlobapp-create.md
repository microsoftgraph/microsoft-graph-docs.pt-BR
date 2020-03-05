---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3d84f87b9602eb6df917729d1d45c69058419e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451095"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="8cc3d-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="8cc3d-103">Create managedAndroidLobApp</span></span>

<span data-ttu-id="8cc3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8cc3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc3d-107">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc3d-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cc3d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8cc3d-108">Prerequisites</span></span>
<span data-ttu-id="8cc3d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cc3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cc3d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cc3d-111">Permission type</span></span>|<span data-ttu-id="8cc3d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cc3d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cc3d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc3d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8cc3d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cc3d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-116">Not supported.</span></span>|
|<span data-ttu-id="8cc3d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cc3d-117">Application</span></span>|<span data-ttu-id="8cc3d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cc3d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cc3d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8cc3d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc3d-120">Request headers</span></span>
|<span data-ttu-id="8cc3d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8cc3d-121">Header</span></span>|<span data-ttu-id="8cc3d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8cc3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cc3d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cc3d-123">Authorization</span></span>|<span data-ttu-id="8cc3d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cc3d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8cc3d-125">Accept</span></span>|<span data-ttu-id="8cc3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cc3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cc3d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc3d-127">Request body</span></span>
<span data-ttu-id="8cc3d-128">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="8cc3d-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="8cc3d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc3d-130">Property</span></span>|<span data-ttu-id="8cc3d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc3d-131">Type</span></span>|<span data-ttu-id="8cc3d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc3d-133">id</span><span class="sxs-lookup"><span data-stu-id="8cc3d-133">id</span></span>|<span data-ttu-id="8cc3d-134">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-134">String</span></span>|<span data-ttu-id="8cc3d-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-135">Key of the entity.</span></span> <span data-ttu-id="8cc3d-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8cc3d-137">displayName</span></span>|<span data-ttu-id="8cc3d-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc3d-138">String</span></span>|<span data-ttu-id="8cc3d-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8cc3d-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-141">description</span><span class="sxs-lookup"><span data-stu-id="8cc3d-141">description</span></span>|<span data-ttu-id="8cc3d-142">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-142">String</span></span>|<span data-ttu-id="8cc3d-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-143">The description of the app.</span></span> <span data-ttu-id="8cc3d-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-145">publicador</span><span class="sxs-lookup"><span data-stu-id="8cc3d-145">publisher</span></span>|<span data-ttu-id="8cc3d-146">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-146">String</span></span>|<span data-ttu-id="8cc3d-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-147">The publisher of the app.</span></span> <span data-ttu-id="8cc3d-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8cc3d-149">largeIcon</span></span>|[<span data-ttu-id="8cc3d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8cc3d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8cc3d-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8cc3d-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc3d-153">createdDateTime</span></span>|<span data-ttu-id="8cc3d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc3d-154">DateTimeOffset</span></span>|<span data-ttu-id="8cc3d-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-155">The date and time the app was created.</span></span> <span data-ttu-id="8cc3d-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc3d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8cc3d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc3d-158">DateTimeOffset</span></span>|<span data-ttu-id="8cc3d-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8cc3d-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8cc3d-161">isFeatured</span></span>|<span data-ttu-id="8cc3d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc3d-162">Boolean</span></span>|<span data-ttu-id="8cc3d-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc3d-164">privacyInformationUrl</span></span>|<span data-ttu-id="8cc3d-165">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-165">String</span></span>|<span data-ttu-id="8cc3d-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-166">The privacy statement Url.</span></span> <span data-ttu-id="8cc3d-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8cc3d-168">informationUrl</span></span>|<span data-ttu-id="8cc3d-169">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-169">String</span></span>|<span data-ttu-id="8cc3d-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-170">The more information Url.</span></span> <span data-ttu-id="8cc3d-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-172">owner</span><span class="sxs-lookup"><span data-stu-id="8cc3d-172">owner</span></span>|<span data-ttu-id="8cc3d-173">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-173">String</span></span>|<span data-ttu-id="8cc3d-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-174">The owner of the app.</span></span> <span data-ttu-id="8cc3d-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-176">developer</span><span class="sxs-lookup"><span data-stu-id="8cc3d-176">developer</span></span>|<span data-ttu-id="8cc3d-177">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-177">String</span></span>|<span data-ttu-id="8cc3d-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-178">The developer of the app.</span></span> <span data-ttu-id="8cc3d-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-180">notes</span><span class="sxs-lookup"><span data-stu-id="8cc3d-180">notes</span></span>|<span data-ttu-id="8cc3d-181">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-181">String</span></span>|<span data-ttu-id="8cc3d-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-182">Notes for the app.</span></span> <span data-ttu-id="8cc3d-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8cc3d-184">uploadState</span></span>|<span data-ttu-id="8cc3d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc3d-185">Int32</span></span>|<span data-ttu-id="8cc3d-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-186">The upload state.</span></span> <span data-ttu-id="8cc3d-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8cc3d-188">publishingState</span></span>|[<span data-ttu-id="8cc3d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8cc3d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8cc3d-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-190">The publishing state for the app.</span></span> <span data-ttu-id="8cc3d-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8cc3d-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc3d-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8cc3d-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8cc3d-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8cc3d-194">isAssigned</span></span>|<span data-ttu-id="8cc3d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cc3d-195">Boolean</span></span>|<span data-ttu-id="8cc3d-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8cc3d-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8cc3d-198">roleScopeTagIds</span></span>|<span data-ttu-id="8cc3d-199">String collection</span><span class="sxs-lookup"><span data-stu-id="8cc3d-199">String collection</span></span>|<span data-ttu-id="8cc3d-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8cc3d-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8cc3d-202">dependentAppCount</span></span>|<span data-ttu-id="8cc3d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc3d-203">Int32</span></span>|<span data-ttu-id="8cc3d-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8cc3d-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8cc3d-206">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8cc3d-206">appAvailability</span></span>|[<span data-ttu-id="8cc3d-207">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8cc3d-207">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8cc3d-208">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-208">The Application's availability.</span></span> <span data-ttu-id="8cc3d-209">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="8cc3d-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8cc3d-210">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-210">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8cc3d-211">version</span><span class="sxs-lookup"><span data-stu-id="8cc3d-211">version</span></span>|<span data-ttu-id="8cc3d-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8cc3d-212">String</span></span>|<span data-ttu-id="8cc3d-213">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-213">The Application's version.</span></span> <span data-ttu-id="8cc3d-214">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-214">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8cc3d-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8cc3d-215">committedContentVersion</span></span>|<span data-ttu-id="8cc3d-216">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-216">String</span></span>|<span data-ttu-id="8cc3d-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-217">The internal committed content version.</span></span> <span data-ttu-id="8cc3d-218">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc3d-219">fileName</span><span class="sxs-lookup"><span data-stu-id="8cc3d-219">fileName</span></span>|<span data-ttu-id="8cc3d-220">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-220">String</span></span>|<span data-ttu-id="8cc3d-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-221">The name of the main Lob application file.</span></span> <span data-ttu-id="8cc3d-222">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc3d-223">size</span><span class="sxs-lookup"><span data-stu-id="8cc3d-223">size</span></span>|<span data-ttu-id="8cc3d-224">Int64</span><span class="sxs-lookup"><span data-stu-id="8cc3d-224">Int64</span></span>|<span data-ttu-id="8cc3d-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="8cc3d-226">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8cc3d-226">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8cc3d-227">packageId</span><span class="sxs-lookup"><span data-stu-id="8cc3d-227">packageId</span></span>|<span data-ttu-id="8cc3d-228">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-228">String</span></span>|<span data-ttu-id="8cc3d-229">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-229">The package identifier.</span></span>|
|<span data-ttu-id="8cc3d-230">identityName</span><span class="sxs-lookup"><span data-stu-id="8cc3d-230">identityName</span></span>|<span data-ttu-id="8cc3d-231">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-231">String</span></span>|<span data-ttu-id="8cc3d-232">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-232">The Identity Name.</span></span>|
|<span data-ttu-id="8cc3d-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc3d-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8cc3d-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8cc3d-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8cc3d-235">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8cc3d-236">versionName</span><span class="sxs-lookup"><span data-stu-id="8cc3d-236">versionName</span></span>|<span data-ttu-id="8cc3d-237">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-237">String</span></span>|<span data-ttu-id="8cc3d-238">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-238">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8cc3d-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="8cc3d-239">versionCode</span></span>|<span data-ttu-id="8cc3d-240">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-240">String</span></span>|<span data-ttu-id="8cc3d-241">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-241">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8cc3d-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="8cc3d-242">identityVersion</span></span>|<span data-ttu-id="8cc3d-243">String</span><span class="sxs-lookup"><span data-stu-id="8cc3d-243">String</span></span>|<span data-ttu-id="8cc3d-244">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="8cc3d-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc3d-245">Response</span></span>
<span data-ttu-id="8cc3d-246">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-246">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cc3d-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cc3d-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cc3d-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cc3d-248">Request</span></span>
<span data-ttu-id="8cc3d-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8cc3d-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cc3d-250">Response</span></span>
<span data-ttu-id="8cc3d-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cc3d-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





