---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b4ce9980b60bf6d6208a005c64bd6dbd8f85234e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961893"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="6cf6b-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="6cf6b-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="6cf6b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cf6b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cf6b-106">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf6b-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cf6b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cf6b-107">Prerequisites</span></span>
<span data-ttu-id="6cf6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cf6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cf6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cf6b-110">Permission type</span></span>|<span data-ttu-id="6cf6b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cf6b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cf6b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cf6b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cf6b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cf6b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-115">Not supported.</span></span>|
|<span data-ttu-id="6cf6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cf6b-116">Application</span></span>|<span data-ttu-id="6cf6b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cf6b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cf6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6cf6b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf6b-119">Request headers</span></span>
|<span data-ttu-id="6cf6b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cf6b-120">Header</span></span>|<span data-ttu-id="6cf6b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6cf6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cf6b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cf6b-122">Authorization</span></span>|<span data-ttu-id="6cf6b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cf6b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cf6b-124">Accept</span></span>|<span data-ttu-id="6cf6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cf6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cf6b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf6b-126">Request body</span></span>
<span data-ttu-id="6cf6b-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="6cf6b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="6cf6b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cf6b-129">Property</span></span>|<span data-ttu-id="6cf6b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cf6b-130">Type</span></span>|<span data-ttu-id="6cf6b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cf6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cf6b-132">id</span><span class="sxs-lookup"><span data-stu-id="6cf6b-132">id</span></span>|<span data-ttu-id="6cf6b-133">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-133">String</span></span>|<span data-ttu-id="6cf6b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-134">Key of the entity.</span></span> <span data-ttu-id="6cf6b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6cf6b-136">displayName</span></span>|<span data-ttu-id="6cf6b-137">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-137">String</span></span>|<span data-ttu-id="6cf6b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6cf6b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-140">descrição</span><span class="sxs-lookup"><span data-stu-id="6cf6b-140">description</span></span>|<span data-ttu-id="6cf6b-141">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-141">String</span></span>|<span data-ttu-id="6cf6b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-142">The description of the app.</span></span> <span data-ttu-id="6cf6b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="6cf6b-144">publisher</span></span>|<span data-ttu-id="6cf6b-145">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-145">String</span></span>|<span data-ttu-id="6cf6b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-146">The publisher of the app.</span></span> <span data-ttu-id="6cf6b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6cf6b-148">largeIcon</span></span>|[<span data-ttu-id="6cf6b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6cf6b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6cf6b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6cf6b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf6b-152">createdDateTime</span></span>|<span data-ttu-id="6cf6b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf6b-153">DateTimeOffset</span></span>|<span data-ttu-id="6cf6b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-154">The date and time the app was created.</span></span> <span data-ttu-id="6cf6b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cf6b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6cf6b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cf6b-157">DateTimeOffset</span></span>|<span data-ttu-id="6cf6b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6cf6b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6cf6b-160">isFeatured</span></span>|<span data-ttu-id="6cf6b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf6b-161">Boolean</span></span>|<span data-ttu-id="6cf6b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6cf6b-163">privacyInformationUrl</span></span>|<span data-ttu-id="6cf6b-164">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-164">String</span></span>|<span data-ttu-id="6cf6b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-165">The privacy statement Url.</span></span> <span data-ttu-id="6cf6b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6cf6b-167">informationUrl</span></span>|<span data-ttu-id="6cf6b-168">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-168">String</span></span>|<span data-ttu-id="6cf6b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-169">The more information Url.</span></span> <span data-ttu-id="6cf6b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-171">owner</span><span class="sxs-lookup"><span data-stu-id="6cf6b-171">owner</span></span>|<span data-ttu-id="6cf6b-172">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-172">String</span></span>|<span data-ttu-id="6cf6b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-173">The owner of the app.</span></span> <span data-ttu-id="6cf6b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-175">developer</span><span class="sxs-lookup"><span data-stu-id="6cf6b-175">developer</span></span>|<span data-ttu-id="6cf6b-176">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-176">String</span></span>|<span data-ttu-id="6cf6b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-177">The developer of the app.</span></span> <span data-ttu-id="6cf6b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-179">notes</span><span class="sxs-lookup"><span data-stu-id="6cf6b-179">notes</span></span>|<span data-ttu-id="6cf6b-180">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-180">String</span></span>|<span data-ttu-id="6cf6b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-181">Notes for the app.</span></span> <span data-ttu-id="6cf6b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6cf6b-183">uploadState</span></span>|<span data-ttu-id="6cf6b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf6b-184">Int32</span></span>|<span data-ttu-id="6cf6b-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-185">The upload state.</span></span> <span data-ttu-id="6cf6b-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6cf6b-187">publishingState</span></span>|[<span data-ttu-id="6cf6b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6cf6b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6cf6b-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-189">The publishing state for the app.</span></span> <span data-ttu-id="6cf6b-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6cf6b-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf6b-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6cf6b-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6cf6b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6cf6b-193">isAssigned</span></span>|<span data-ttu-id="6cf6b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cf6b-194">Boolean</span></span>|<span data-ttu-id="6cf6b-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6cf6b-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cf6b-197">roleScopeTagIds</span></span>|<span data-ttu-id="6cf6b-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cf6b-198">String collection</span></span>|<span data-ttu-id="6cf6b-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6cf6b-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6cf6b-201">dependentAppCount</span></span>|<span data-ttu-id="6cf6b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6cf6b-202">Int32</span></span>|<span data-ttu-id="6cf6b-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6cf6b-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cf6b-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="6cf6b-205">appAvailability</span></span>|[<span data-ttu-id="6cf6b-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="6cf6b-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="6cf6b-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-207">The Application's availability.</span></span> <span data-ttu-id="6cf6b-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cf6b-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="6cf6b-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="6cf6b-210">version</span><span class="sxs-lookup"><span data-stu-id="6cf6b-210">version</span></span>|<span data-ttu-id="6cf6b-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cf6b-211">String</span></span>|<span data-ttu-id="6cf6b-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-212">The Application's version.</span></span> <span data-ttu-id="6cf6b-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="6cf6b-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6cf6b-214">committedContentVersion</span></span>|<span data-ttu-id="6cf6b-215">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-215">String</span></span>|<span data-ttu-id="6cf6b-216">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-216">The internal committed content version.</span></span> <span data-ttu-id="6cf6b-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6cf6b-218">fileName</span><span class="sxs-lookup"><span data-stu-id="6cf6b-218">fileName</span></span>|<span data-ttu-id="6cf6b-219">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-219">String</span></span>|<span data-ttu-id="6cf6b-220">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-220">The name of the main Lob application file.</span></span> <span data-ttu-id="6cf6b-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6cf6b-222">size</span><span class="sxs-lookup"><span data-stu-id="6cf6b-222">size</span></span>|<span data-ttu-id="6cf6b-223">Int64</span><span class="sxs-lookup"><span data-stu-id="6cf6b-223">Int64</span></span>|<span data-ttu-id="6cf6b-224">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="6cf6b-225">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cf6b-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="6cf6b-226">packageId</span><span class="sxs-lookup"><span data-stu-id="6cf6b-226">packageId</span></span>|<span data-ttu-id="6cf6b-227">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-227">String</span></span>|<span data-ttu-id="6cf6b-228">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-228">The package identifier.</span></span>|
|<span data-ttu-id="6cf6b-229">identityName</span><span class="sxs-lookup"><span data-stu-id="6cf6b-229">identityName</span></span>|<span data-ttu-id="6cf6b-230">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-230">String</span></span>|<span data-ttu-id="6cf6b-231">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-231">The Identity Name.</span></span>|
|<span data-ttu-id="6cf6b-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6cf6b-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6cf6b-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6cf6b-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="6cf6b-234">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="6cf6b-235">versionName</span><span class="sxs-lookup"><span data-stu-id="6cf6b-235">versionName</span></span>|<span data-ttu-id="6cf6b-236">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-236">String</span></span>|<span data-ttu-id="6cf6b-237">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6cf6b-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="6cf6b-238">versionCode</span></span>|<span data-ttu-id="6cf6b-239">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-239">String</span></span>|<span data-ttu-id="6cf6b-240">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="6cf6b-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6cf6b-241">identityVersion</span></span>|<span data-ttu-id="6cf6b-242">String</span><span class="sxs-lookup"><span data-stu-id="6cf6b-242">String</span></span>|<span data-ttu-id="6cf6b-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="6cf6b-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf6b-244">Response</span></span>
<span data-ttu-id="6cf6b-245">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-245">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cf6b-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cf6b-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cf6b-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cf6b-247">Request</span></span>
<span data-ttu-id="6cf6b-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cf6b-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cf6b-249">Response</span></span>
<span data-ttu-id="6cf6b-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cf6b-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





