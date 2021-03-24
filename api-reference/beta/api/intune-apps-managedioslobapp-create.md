---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ed108887b50a25ef7333f3aeebe7feff4ea031d2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143525"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="bfdee-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="bfdee-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="bfdee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfdee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfdee-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bfdee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfdee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bfdee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfdee-107">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfdee-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bfdee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bfdee-108">Prerequisites</span></span>
<span data-ttu-id="bfdee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfdee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bfdee-111">Permission type</span></span>|<span data-ttu-id="bfdee-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bfdee-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bfdee-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bfdee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bfdee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bfdee-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bfdee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bfdee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bfdee-116">Not supported.</span></span>|
|<span data-ttu-id="bfdee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bfdee-117">Application</span></span>|<span data-ttu-id="bfdee-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfdee-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bfdee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bfdee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bfdee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bfdee-120">Request headers</span></span>
|<span data-ttu-id="bfdee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bfdee-121">Header</span></span>|<span data-ttu-id="bfdee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bfdee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bfdee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bfdee-123">Authorization</span></span>|<span data-ttu-id="bfdee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bfdee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bfdee-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bfdee-125">Accept</span></span>|<span data-ttu-id="bfdee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bfdee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bfdee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bfdee-127">Request body</span></span>
<span data-ttu-id="bfdee-128">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="bfdee-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="bfdee-129">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="bfdee-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="bfdee-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bfdee-130">Property</span></span>|<span data-ttu-id="bfdee-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfdee-131">Type</span></span>|<span data-ttu-id="bfdee-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfdee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfdee-133">id</span><span class="sxs-lookup"><span data-stu-id="bfdee-133">id</span></span>|<span data-ttu-id="bfdee-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfdee-134">String</span></span>|<span data-ttu-id="bfdee-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bfdee-135">Key of the entity.</span></span> <span data-ttu-id="bfdee-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bfdee-137">displayName</span></span>|<span data-ttu-id="bfdee-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfdee-138">String</span></span>|<span data-ttu-id="bfdee-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="bfdee-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bfdee-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-141">descrição</span><span class="sxs-lookup"><span data-stu-id="bfdee-141">description</span></span>|<span data-ttu-id="bfdee-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfdee-142">String</span></span>|<span data-ttu-id="bfdee-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-143">The description of the app.</span></span> <span data-ttu-id="bfdee-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-145">publicador</span><span class="sxs-lookup"><span data-stu-id="bfdee-145">publisher</span></span>|<span data-ttu-id="bfdee-146">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-146">String</span></span>|<span data-ttu-id="bfdee-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-147">The publisher of the app.</span></span> <span data-ttu-id="bfdee-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bfdee-149">largeIcon</span></span>|[<span data-ttu-id="bfdee-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bfdee-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bfdee-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="bfdee-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bfdee-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdee-153">createdDateTime</span></span>|<span data-ttu-id="bfdee-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdee-154">DateTimeOffset</span></span>|<span data-ttu-id="bfdee-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-155">The date and time the app was created.</span></span> <span data-ttu-id="bfdee-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdee-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bfdee-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdee-158">DateTimeOffset</span></span>|<span data-ttu-id="bfdee-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="bfdee-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bfdee-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bfdee-161">isFeatured</span></span>|<span data-ttu-id="bfdee-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdee-162">Boolean</span></span>|<span data-ttu-id="bfdee-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bfdee-164">privacyInformationUrl</span></span>|<span data-ttu-id="bfdee-165">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-165">String</span></span>|<span data-ttu-id="bfdee-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="bfdee-166">The privacy statement Url.</span></span> <span data-ttu-id="bfdee-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bfdee-168">informationUrl</span></span>|<span data-ttu-id="bfdee-169">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-169">String</span></span>|<span data-ttu-id="bfdee-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="bfdee-170">The more information Url.</span></span> <span data-ttu-id="bfdee-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-172">owner</span><span class="sxs-lookup"><span data-stu-id="bfdee-172">owner</span></span>|<span data-ttu-id="bfdee-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfdee-173">String</span></span>|<span data-ttu-id="bfdee-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-174">The owner of the app.</span></span> <span data-ttu-id="bfdee-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-176">developer</span><span class="sxs-lookup"><span data-stu-id="bfdee-176">developer</span></span>|<span data-ttu-id="bfdee-177">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-177">String</span></span>|<span data-ttu-id="bfdee-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-178">The developer of the app.</span></span> <span data-ttu-id="bfdee-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-180">notes</span><span class="sxs-lookup"><span data-stu-id="bfdee-180">notes</span></span>|<span data-ttu-id="bfdee-181">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-181">String</span></span>|<span data-ttu-id="bfdee-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-182">Notes for the app.</span></span> <span data-ttu-id="bfdee-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bfdee-184">uploadState</span></span>|<span data-ttu-id="bfdee-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdee-185">Int32</span></span>|<span data-ttu-id="bfdee-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="bfdee-186">The upload state.</span></span> <span data-ttu-id="bfdee-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="bfdee-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bfdee-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bfdee-189">publishingState</span></span>|[<span data-ttu-id="bfdee-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bfdee-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bfdee-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-191">The publishing state for the app.</span></span> <span data-ttu-id="bfdee-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="bfdee-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bfdee-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfdee-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bfdee-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="bfdee-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bfdee-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bfdee-195">isAssigned</span></span>|<span data-ttu-id="bfdee-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bfdee-196">Boolean</span></span>|<span data-ttu-id="bfdee-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bfdee-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bfdee-199">roleScopeTagIds</span></span>|<span data-ttu-id="bfdee-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bfdee-200">String collection</span></span>|<span data-ttu-id="bfdee-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="bfdee-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bfdee-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bfdee-203">dependentAppCount</span></span>|<span data-ttu-id="bfdee-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdee-204">Int32</span></span>|<span data-ttu-id="bfdee-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="bfdee-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bfdee-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="bfdee-207">supersedingAppCount</span></span>|<span data-ttu-id="bfdee-208">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdee-208">Int32</span></span>|<span data-ttu-id="bfdee-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="bfdee-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="bfdee-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="bfdee-211">supersededAppCount</span></span>|<span data-ttu-id="bfdee-212">Int32</span><span class="sxs-lookup"><span data-stu-id="bfdee-212">Int32</span></span>|<span data-ttu-id="bfdee-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="bfdee-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="bfdee-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bfdee-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="bfdee-215">appAvailability</span></span>|[<span data-ttu-id="bfdee-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="bfdee-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="bfdee-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-217">The Application's availability.</span></span> <span data-ttu-id="bfdee-218">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bfdee-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="bfdee-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="bfdee-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="bfdee-220">version</span><span class="sxs-lookup"><span data-stu-id="bfdee-220">version</span></span>|<span data-ttu-id="bfdee-221">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-221">String</span></span>|<span data-ttu-id="bfdee-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bfdee-222">The Application's version.</span></span> <span data-ttu-id="bfdee-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="bfdee-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bfdee-224">committedContentVersion</span></span>|<span data-ttu-id="bfdee-225">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-225">String</span></span>|<span data-ttu-id="bfdee-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="bfdee-226">The internal committed content version.</span></span> <span data-ttu-id="bfdee-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bfdee-228">fileName</span><span class="sxs-lookup"><span data-stu-id="bfdee-228">fileName</span></span>|<span data-ttu-id="bfdee-229">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-229">String</span></span>|<span data-ttu-id="bfdee-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="bfdee-230">The name of the main Lob application file.</span></span> <span data-ttu-id="bfdee-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bfdee-232">size</span><span class="sxs-lookup"><span data-stu-id="bfdee-232">size</span></span>|<span data-ttu-id="bfdee-233">Int64</span><span class="sxs-lookup"><span data-stu-id="bfdee-233">Int64</span></span>|<span data-ttu-id="bfdee-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="bfdee-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="bfdee-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bfdee-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="bfdee-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="bfdee-236">bundleId</span></span>|<span data-ttu-id="bfdee-237">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-237">String</span></span>|<span data-ttu-id="bfdee-238">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="bfdee-238">The Identity Name.</span></span>|
|<span data-ttu-id="bfdee-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="bfdee-239">applicableDeviceType</span></span>|[<span data-ttu-id="bfdee-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="bfdee-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="bfdee-241">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="bfdee-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="bfdee-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bfdee-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bfdee-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bfdee-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="bfdee-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="bfdee-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bfdee-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bfdee-245">expirationDateTime</span></span>|<span data-ttu-id="bfdee-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfdee-246">DateTimeOffset</span></span>|<span data-ttu-id="bfdee-247">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="bfdee-247">The expiration time.</span></span>|
|<span data-ttu-id="bfdee-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="bfdee-248">versionNumber</span></span>|<span data-ttu-id="bfdee-249">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-249">String</span></span>|<span data-ttu-id="bfdee-250">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bfdee-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bfdee-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="bfdee-251">buildNumber</span></span>|<span data-ttu-id="bfdee-252">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-252">String</span></span>|<span data-ttu-id="bfdee-253">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="bfdee-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bfdee-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bfdee-254">identityVersion</span></span>|<span data-ttu-id="bfdee-255">String</span><span class="sxs-lookup"><span data-stu-id="bfdee-255">String</span></span>|<span data-ttu-id="bfdee-256">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="bfdee-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="bfdee-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfdee-257">Response</span></span>
<span data-ttu-id="bfdee-258">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bfdee-258">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfdee-259">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bfdee-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="bfdee-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bfdee-260">Request</span></span>
<span data-ttu-id="bfdee-261">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bfdee-261">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1566

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="bfdee-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="bfdee-262">Response</span></span>
<span data-ttu-id="bfdee-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bfdee-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1738

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




