---
title: Atualizar managedIOSLobApp
description: Atualiza as propriedades de um objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2fbf159f0b9b8acc65218ce60263cb2e277001d0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143518"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="1bb88-103">Atualizar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="1bb88-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="1bb88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1bb88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1bb88-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1bb88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1bb88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1bb88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bb88-107">Atualiza as propriedades de um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bb88-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bb88-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1bb88-108">Prerequisites</span></span>
<span data-ttu-id="1bb88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb88-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1bb88-111">Permission type</span></span>|<span data-ttu-id="1bb88-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1bb88-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bb88-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1bb88-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1bb88-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb88-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bb88-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1bb88-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bb88-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1bb88-116">Not supported.</span></span>|
|<span data-ttu-id="1bb88-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1bb88-117">Application</span></span>|<span data-ttu-id="1bb88-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb88-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bb88-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1bb88-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1bb88-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb88-120">Request headers</span></span>
|<span data-ttu-id="1bb88-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1bb88-121">Header</span></span>|<span data-ttu-id="1bb88-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1bb88-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bb88-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1bb88-123">Authorization</span></span>|<span data-ttu-id="1bb88-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1bb88-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bb88-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1bb88-125">Accept</span></span>|<span data-ttu-id="1bb88-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1bb88-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bb88-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb88-127">Request body</span></span>
<span data-ttu-id="1bb88-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bb88-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="1bb88-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bb88-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="1bb88-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1bb88-130">Property</span></span>|<span data-ttu-id="1bb88-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1bb88-131">Type</span></span>|<span data-ttu-id="1bb88-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1bb88-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bb88-133">id</span><span class="sxs-lookup"><span data-stu-id="1bb88-133">id</span></span>|<span data-ttu-id="1bb88-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bb88-134">String</span></span>|<span data-ttu-id="1bb88-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1bb88-135">Key of the entity.</span></span> <span data-ttu-id="1bb88-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1bb88-137">displayName</span></span>|<span data-ttu-id="1bb88-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bb88-138">String</span></span>|<span data-ttu-id="1bb88-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1bb88-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1bb88-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-141">descrição</span><span class="sxs-lookup"><span data-stu-id="1bb88-141">description</span></span>|<span data-ttu-id="1bb88-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bb88-142">String</span></span>|<span data-ttu-id="1bb88-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-143">The description of the app.</span></span> <span data-ttu-id="1bb88-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-145">publicador</span><span class="sxs-lookup"><span data-stu-id="1bb88-145">publisher</span></span>|<span data-ttu-id="1bb88-146">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-146">String</span></span>|<span data-ttu-id="1bb88-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-147">The publisher of the app.</span></span> <span data-ttu-id="1bb88-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1bb88-149">largeIcon</span></span>|[<span data-ttu-id="1bb88-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1bb88-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1bb88-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1bb88-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1bb88-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb88-153">createdDateTime</span></span>|<span data-ttu-id="1bb88-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb88-154">DateTimeOffset</span></span>|<span data-ttu-id="1bb88-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-155">The date and time the app was created.</span></span> <span data-ttu-id="1bb88-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb88-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1bb88-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb88-158">DateTimeOffset</span></span>|<span data-ttu-id="1bb88-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1bb88-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1bb88-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1bb88-161">isFeatured</span></span>|<span data-ttu-id="1bb88-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bb88-162">Boolean</span></span>|<span data-ttu-id="1bb88-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1bb88-164">privacyInformationUrl</span></span>|<span data-ttu-id="1bb88-165">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-165">String</span></span>|<span data-ttu-id="1bb88-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1bb88-166">The privacy statement Url.</span></span> <span data-ttu-id="1bb88-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1bb88-168">informationUrl</span></span>|<span data-ttu-id="1bb88-169">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-169">String</span></span>|<span data-ttu-id="1bb88-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1bb88-170">The more information Url.</span></span> <span data-ttu-id="1bb88-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-172">owner</span><span class="sxs-lookup"><span data-stu-id="1bb88-172">owner</span></span>|<span data-ttu-id="1bb88-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bb88-173">String</span></span>|<span data-ttu-id="1bb88-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-174">The owner of the app.</span></span> <span data-ttu-id="1bb88-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-176">developer</span><span class="sxs-lookup"><span data-stu-id="1bb88-176">developer</span></span>|<span data-ttu-id="1bb88-177">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-177">String</span></span>|<span data-ttu-id="1bb88-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-178">The developer of the app.</span></span> <span data-ttu-id="1bb88-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-180">notes</span><span class="sxs-lookup"><span data-stu-id="1bb88-180">notes</span></span>|<span data-ttu-id="1bb88-181">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-181">String</span></span>|<span data-ttu-id="1bb88-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-182">Notes for the app.</span></span> <span data-ttu-id="1bb88-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1bb88-184">uploadState</span></span>|<span data-ttu-id="1bb88-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb88-185">Int32</span></span>|<span data-ttu-id="1bb88-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="1bb88-186">The upload state.</span></span> <span data-ttu-id="1bb88-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="1bb88-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="1bb88-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="1bb88-189">publishingState</span></span>|[<span data-ttu-id="1bb88-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1bb88-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1bb88-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-191">The publishing state for the app.</span></span> <span data-ttu-id="1bb88-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1bb88-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1bb88-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bb88-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1bb88-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1bb88-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1bb88-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1bb88-195">isAssigned</span></span>|<span data-ttu-id="1bb88-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bb88-196">Boolean</span></span>|<span data-ttu-id="1bb88-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1bb88-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1bb88-199">roleScopeTagIds</span></span>|<span data-ttu-id="1bb88-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1bb88-200">String collection</span></span>|<span data-ttu-id="1bb88-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1bb88-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1bb88-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1bb88-203">dependentAppCount</span></span>|<span data-ttu-id="1bb88-204">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb88-204">Int32</span></span>|<span data-ttu-id="1bb88-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="1bb88-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1bb88-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="1bb88-207">supersedingAppCount</span></span>|<span data-ttu-id="1bb88-208">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb88-208">Int32</span></span>|<span data-ttu-id="1bb88-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="1bb88-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="1bb88-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="1bb88-211">supersededAppCount</span></span>|<span data-ttu-id="1bb88-212">Int32</span><span class="sxs-lookup"><span data-stu-id="1bb88-212">Int32</span></span>|<span data-ttu-id="1bb88-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="1bb88-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="1bb88-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1bb88-215">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1bb88-215">appAvailability</span></span>|[<span data-ttu-id="1bb88-216">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="1bb88-216">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="1bb88-217">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-217">The Application's availability.</span></span> <span data-ttu-id="1bb88-218">Herdado [de managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="1bb88-218">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="1bb88-219">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="1bb88-219">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1bb88-220">version</span><span class="sxs-lookup"><span data-stu-id="1bb88-220">version</span></span>|<span data-ttu-id="1bb88-221">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-221">String</span></span>|<span data-ttu-id="1bb88-222">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1bb88-222">The Application's version.</span></span> <span data-ttu-id="1bb88-223">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-223">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="1bb88-224">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1bb88-224">committedContentVersion</span></span>|<span data-ttu-id="1bb88-225">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-225">String</span></span>|<span data-ttu-id="1bb88-226">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="1bb88-226">The internal committed content version.</span></span> <span data-ttu-id="1bb88-227">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-227">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb88-228">fileName</span><span class="sxs-lookup"><span data-stu-id="1bb88-228">fileName</span></span>|<span data-ttu-id="1bb88-229">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-229">String</span></span>|<span data-ttu-id="1bb88-230">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="1bb88-230">The name of the main Lob application file.</span></span> <span data-ttu-id="1bb88-231">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-231">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb88-232">size</span><span class="sxs-lookup"><span data-stu-id="1bb88-232">size</span></span>|<span data-ttu-id="1bb88-233">Int64</span><span class="sxs-lookup"><span data-stu-id="1bb88-233">Int64</span></span>|<span data-ttu-id="1bb88-234">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="1bb88-234">The total size, including all uploaded files.</span></span> <span data-ttu-id="1bb88-235">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1bb88-235">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1bb88-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="1bb88-236">bundleId</span></span>|<span data-ttu-id="1bb88-237">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-237">String</span></span>|<span data-ttu-id="1bb88-238">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb88-238">The Identity Name.</span></span>|
|<span data-ttu-id="1bb88-239">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1bb88-239">applicableDeviceType</span></span>|[<span data-ttu-id="1bb88-240">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1bb88-240">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1bb88-241">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1bb88-241">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1bb88-242">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1bb88-242">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1bb88-243">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1bb88-243">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1bb88-244">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1bb88-244">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1bb88-245">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1bb88-245">expirationDateTime</span></span>|<span data-ttu-id="1bb88-246">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bb88-246">DateTimeOffset</span></span>|<span data-ttu-id="1bb88-247">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="1bb88-247">The expiration time.</span></span>|
|<span data-ttu-id="1bb88-248">versionNumber</span><span class="sxs-lookup"><span data-stu-id="1bb88-248">versionNumber</span></span>|<span data-ttu-id="1bb88-249">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-249">String</span></span>|<span data-ttu-id="1bb88-250">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="1bb88-250">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1bb88-251">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1bb88-251">buildNumber</span></span>|<span data-ttu-id="1bb88-252">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-252">String</span></span>|<span data-ttu-id="1bb88-253">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="1bb88-253">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1bb88-254">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1bb88-254">identityVersion</span></span>|<span data-ttu-id="1bb88-255">String</span><span class="sxs-lookup"><span data-stu-id="1bb88-255">String</span></span>|<span data-ttu-id="1bb88-256">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="1bb88-256">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1bb88-257">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb88-257">Response</span></span>
<span data-ttu-id="1bb88-258">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1bb88-258">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bb88-259">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1bb88-259">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bb88-260">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1bb88-260">Request</span></span>
<span data-ttu-id="1bb88-261">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1bb88-261">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="1bb88-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="1bb88-262">Response</span></span>
<span data-ttu-id="1bb88-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1bb88-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




