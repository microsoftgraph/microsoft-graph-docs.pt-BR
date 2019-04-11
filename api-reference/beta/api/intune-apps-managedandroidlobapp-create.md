---
title: Criar managedAndroidLobApp
description: Cria um novo objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e99e21e2cbc558cb8d482298224e79a60fc1aea
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783511"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="d91ab-103">Criar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="d91ab-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="d91ab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d91ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d91ab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d91ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d91ab-106">Cria um novo objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d91ab-106">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d91ab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d91ab-107">Prerequisites</span></span>
<span data-ttu-id="d91ab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d91ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d91ab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d91ab-110">Permission type</span></span>|<span data-ttu-id="d91ab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d91ab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d91ab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d91ab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d91ab-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d91ab-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d91ab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d91ab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d91ab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d91ab-115">Not supported.</span></span>|
|<span data-ttu-id="d91ab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d91ab-116">Application</span></span>|<span data-ttu-id="d91ab-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d91ab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d91ab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d91ab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d91ab-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ab-119">Request headers</span></span>
|<span data-ttu-id="d91ab-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d91ab-120">Header</span></span>|<span data-ttu-id="d91ab-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d91ab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d91ab-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d91ab-122">Authorization</span></span>|<span data-ttu-id="d91ab-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d91ab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d91ab-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d91ab-124">Accept</span></span>|<span data-ttu-id="d91ab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d91ab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d91ab-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ab-126">Request body</span></span>
<span data-ttu-id="d91ab-127">No corpo da solicitação, forneça uma representação JSON do objeto managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d91ab-127">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="d91ab-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="d91ab-128">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="d91ab-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d91ab-129">Property</span></span>|<span data-ttu-id="d91ab-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d91ab-130">Type</span></span>|<span data-ttu-id="d91ab-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d91ab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d91ab-132">id</span><span class="sxs-lookup"><span data-stu-id="d91ab-132">id</span></span>|<span data-ttu-id="d91ab-133">String</span><span class="sxs-lookup"><span data-stu-id="d91ab-133">String</span></span>|<span data-ttu-id="d91ab-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d91ab-134">Key of the entity.</span></span> <span data-ttu-id="d91ab-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d91ab-136">displayName</span></span>|<span data-ttu-id="d91ab-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-137">String</span></span>|<span data-ttu-id="d91ab-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="d91ab-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d91ab-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-140">description</span><span class="sxs-lookup"><span data-stu-id="d91ab-140">description</span></span>|<span data-ttu-id="d91ab-141">String</span><span class="sxs-lookup"><span data-stu-id="d91ab-141">String</span></span>|<span data-ttu-id="d91ab-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-142">The description of the app.</span></span> <span data-ttu-id="d91ab-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-144">publicador</span><span class="sxs-lookup"><span data-stu-id="d91ab-144">publisher</span></span>|<span data-ttu-id="d91ab-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-145">String</span></span>|<span data-ttu-id="d91ab-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-146">The publisher of the app.</span></span> <span data-ttu-id="d91ab-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d91ab-148">largeIcon</span></span>|[<span data-ttu-id="d91ab-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d91ab-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d91ab-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="d91ab-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d91ab-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d91ab-152">createdDateTime</span></span>|<span data-ttu-id="d91ab-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d91ab-153">DateTimeOffset</span></span>|<span data-ttu-id="d91ab-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-154">The date and time the app was created.</span></span> <span data-ttu-id="d91ab-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d91ab-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d91ab-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d91ab-157">DateTimeOffset</span></span>|<span data-ttu-id="d91ab-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="d91ab-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d91ab-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d91ab-160">isFeatured</span></span>|<span data-ttu-id="d91ab-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d91ab-161">Boolean</span></span>|<span data-ttu-id="d91ab-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d91ab-163">privacyInformationUrl</span></span>|<span data-ttu-id="d91ab-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-164">String</span></span>|<span data-ttu-id="d91ab-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="d91ab-165">The privacy statement Url.</span></span> <span data-ttu-id="d91ab-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d91ab-167">informationUrl</span></span>|<span data-ttu-id="d91ab-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-168">String</span></span>|<span data-ttu-id="d91ab-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="d91ab-169">The more information Url.</span></span> <span data-ttu-id="d91ab-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-171">owner</span><span class="sxs-lookup"><span data-stu-id="d91ab-171">owner</span></span>|<span data-ttu-id="d91ab-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-172">String</span></span>|<span data-ttu-id="d91ab-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-173">The owner of the app.</span></span> <span data-ttu-id="d91ab-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-175">developer</span><span class="sxs-lookup"><span data-stu-id="d91ab-175">developer</span></span>|<span data-ttu-id="d91ab-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-176">String</span></span>|<span data-ttu-id="d91ab-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-177">The developer of the app.</span></span> <span data-ttu-id="d91ab-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-179">notes</span><span class="sxs-lookup"><span data-stu-id="d91ab-179">notes</span></span>|<span data-ttu-id="d91ab-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-180">String</span></span>|<span data-ttu-id="d91ab-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-181">Notes for the app.</span></span> <span data-ttu-id="d91ab-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="d91ab-183">uploadState</span></span>|<span data-ttu-id="d91ab-184">Int32</span><span class="sxs-lookup"><span data-stu-id="d91ab-184">Int32</span></span>|<span data-ttu-id="d91ab-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="d91ab-185">The upload state.</span></span> <span data-ttu-id="d91ab-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="d91ab-187">publishingState</span></span>|[<span data-ttu-id="d91ab-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d91ab-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d91ab-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-189">The publishing state for the app.</span></span> <span data-ttu-id="d91ab-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="d91ab-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d91ab-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d91ab-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d91ab-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d91ab-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d91ab-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="d91ab-193">isAssigned</span></span>|<span data-ttu-id="d91ab-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="d91ab-194">Boolean</span></span>|<span data-ttu-id="d91ab-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="d91ab-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d91ab-197">roleScopeTagIds</span></span>|<span data-ttu-id="d91ab-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="d91ab-198">String collection</span></span>|<span data-ttu-id="d91ab-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="d91ab-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="d91ab-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d91ab-201">dependentAppCount</span></span>|<span data-ttu-id="d91ab-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d91ab-202">Int32</span></span>|<span data-ttu-id="d91ab-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="d91ab-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="d91ab-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d91ab-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d91ab-205">appAvailability</span></span>|[<span data-ttu-id="d91ab-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d91ab-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d91ab-207">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-207">The Application's availability.</span></span> <span data-ttu-id="d91ab-208">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="d91ab-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d91ab-209">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="d91ab-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d91ab-210">version</span><span class="sxs-lookup"><span data-stu-id="d91ab-210">version</span></span>|<span data-ttu-id="d91ab-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-211">String</span></span>|<span data-ttu-id="d91ab-212">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d91ab-212">The Application's version.</span></span> <span data-ttu-id="d91ab-213">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d91ab-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d91ab-214">committedContentVersion</span></span>|<span data-ttu-id="d91ab-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-215">String</span></span>|<span data-ttu-id="d91ab-216">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="d91ab-216">The internal committed content version.</span></span> <span data-ttu-id="d91ab-217">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d91ab-218">fileName</span><span class="sxs-lookup"><span data-stu-id="d91ab-218">fileName</span></span>|<span data-ttu-id="d91ab-219">String</span><span class="sxs-lookup"><span data-stu-id="d91ab-219">String</span></span>|<span data-ttu-id="d91ab-220">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="d91ab-220">The name of the main Lob application file.</span></span> <span data-ttu-id="d91ab-221">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d91ab-222">size</span><span class="sxs-lookup"><span data-stu-id="d91ab-222">size</span></span>|<span data-ttu-id="d91ab-223">Int64</span><span class="sxs-lookup"><span data-stu-id="d91ab-223">Int64</span></span>|<span data-ttu-id="d91ab-224">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="d91ab-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="d91ab-225">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d91ab-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d91ab-226">packageId</span><span class="sxs-lookup"><span data-stu-id="d91ab-226">packageId</span></span>|<span data-ttu-id="d91ab-227">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-227">String</span></span>|<span data-ttu-id="d91ab-228">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="d91ab-228">The package identifier.</span></span>|
|<span data-ttu-id="d91ab-229">identityName</span><span class="sxs-lookup"><span data-stu-id="d91ab-229">identityName</span></span>|<span data-ttu-id="d91ab-230">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-230">String</span></span>|<span data-ttu-id="d91ab-231">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="d91ab-231">The Identity Name.</span></span>|
|<span data-ttu-id="d91ab-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d91ab-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d91ab-233">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d91ab-233">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="d91ab-234">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="d91ab-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d91ab-235">versionName</span><span class="sxs-lookup"><span data-stu-id="d91ab-235">versionName</span></span>|<span data-ttu-id="d91ab-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-236">String</span></span>|<span data-ttu-id="d91ab-237">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d91ab-237">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d91ab-238">versionCode</span><span class="sxs-lookup"><span data-stu-id="d91ab-238">versionCode</span></span>|<span data-ttu-id="d91ab-239">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d91ab-239">String</span></span>|<span data-ttu-id="d91ab-240">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="d91ab-240">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d91ab-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d91ab-241">identityVersion</span></span>|<span data-ttu-id="d91ab-242">String</span><span class="sxs-lookup"><span data-stu-id="d91ab-242">String</span></span>|<span data-ttu-id="d91ab-243">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="d91ab-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d91ab-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="d91ab-244">Response</span></span>
<span data-ttu-id="d91ab-245">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d91ab-245">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d91ab-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d91ab-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="d91ab-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d91ab-247">Request</span></span>
<span data-ttu-id="d91ab-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d91ab-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d91ab-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="d91ab-249">Response</span></span>
<span data-ttu-id="d91ab-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d91ab-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





