---
title: Atualizar windowsUniversalAppX
description: Atualiza as propriedades de um objeto windowsUniversalAppX.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c618782342a525f208ffaf9e6aa6a7e00b8b8ee2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133322"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="4a068-103">Atualizar windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="4a068-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="4a068-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a068-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a068-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a068-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a068-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a068-107">Atualiza as propriedades de um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="4a068-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a068-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a068-108">Prerequisites</span></span>
<span data-ttu-id="4a068-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a068-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a068-111">Permission type</span></span>|<span data-ttu-id="4a068-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4a068-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a068-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a068-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4a068-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a068-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4a068-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a068-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a068-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a068-116">Not supported.</span></span>|
|<span data-ttu-id="4a068-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a068-117">Application</span></span>|<span data-ttu-id="4a068-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a068-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a068-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a068-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4a068-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a068-120">Request headers</span></span>
|<span data-ttu-id="4a068-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a068-121">Header</span></span>|<span data-ttu-id="4a068-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4a068-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a068-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a068-123">Authorization</span></span>|<span data-ttu-id="4a068-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a068-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a068-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a068-125">Accept</span></span>|<span data-ttu-id="4a068-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4a068-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a068-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a068-127">Request body</span></span>
<span data-ttu-id="4a068-128">No corpo da solicitação, forneça uma representação JSON do objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="4a068-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="4a068-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span><span class="sxs-lookup"><span data-stu-id="4a068-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="4a068-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a068-130">Property</span></span>|<span data-ttu-id="4a068-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a068-131">Type</span></span>|<span data-ttu-id="4a068-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a068-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a068-133">id</span><span class="sxs-lookup"><span data-stu-id="4a068-133">id</span></span>|<span data-ttu-id="4a068-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a068-134">String</span></span>|<span data-ttu-id="4a068-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-135">Key of the entity.</span></span> <span data-ttu-id="4a068-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4a068-137">displayName</span></span>|<span data-ttu-id="4a068-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a068-138">String</span></span>|<span data-ttu-id="4a068-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4a068-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4a068-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-141">descrição</span><span class="sxs-lookup"><span data-stu-id="4a068-141">description</span></span>|<span data-ttu-id="4a068-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a068-142">String</span></span>|<span data-ttu-id="4a068-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-143">The description of the app.</span></span> <span data-ttu-id="4a068-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4a068-145">publisher</span></span>|<span data-ttu-id="4a068-146">String</span><span class="sxs-lookup"><span data-stu-id="4a068-146">String</span></span>|<span data-ttu-id="4a068-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-147">The publisher of the app.</span></span> <span data-ttu-id="4a068-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4a068-149">largeIcon</span></span>|[<span data-ttu-id="4a068-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4a068-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4a068-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4a068-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4a068-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4a068-153">createdDateTime</span></span>|<span data-ttu-id="4a068-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a068-154">DateTimeOffset</span></span>|<span data-ttu-id="4a068-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-155">The date and time the app was created.</span></span> <span data-ttu-id="4a068-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4a068-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4a068-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a068-158">DateTimeOffset</span></span>|<span data-ttu-id="4a068-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4a068-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4a068-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4a068-161">isFeatured</span></span>|<span data-ttu-id="4a068-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a068-162">Boolean</span></span>|<span data-ttu-id="4a068-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4a068-164">privacyInformationUrl</span></span>|<span data-ttu-id="4a068-165">String</span><span class="sxs-lookup"><span data-stu-id="4a068-165">String</span></span>|<span data-ttu-id="4a068-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-166">The privacy statement Url.</span></span> <span data-ttu-id="4a068-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4a068-168">informationUrl</span></span>|<span data-ttu-id="4a068-169">String</span><span class="sxs-lookup"><span data-stu-id="4a068-169">String</span></span>|<span data-ttu-id="4a068-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4a068-170">The more information Url.</span></span> <span data-ttu-id="4a068-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-172">owner</span><span class="sxs-lookup"><span data-stu-id="4a068-172">owner</span></span>|<span data-ttu-id="4a068-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a068-173">String</span></span>|<span data-ttu-id="4a068-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4a068-174">The owner of the app.</span></span> <span data-ttu-id="4a068-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-176">developer</span><span class="sxs-lookup"><span data-stu-id="4a068-176">developer</span></span>|<span data-ttu-id="4a068-177">String</span><span class="sxs-lookup"><span data-stu-id="4a068-177">String</span></span>|<span data-ttu-id="4a068-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-178">The developer of the app.</span></span> <span data-ttu-id="4a068-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-180">notes</span><span class="sxs-lookup"><span data-stu-id="4a068-180">notes</span></span>|<span data-ttu-id="4a068-181">String</span><span class="sxs-lookup"><span data-stu-id="4a068-181">String</span></span>|<span data-ttu-id="4a068-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-182">Notes for the app.</span></span> <span data-ttu-id="4a068-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4a068-184">uploadState</span></span>|<span data-ttu-id="4a068-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4a068-185">Int32</span></span>|<span data-ttu-id="4a068-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4a068-186">The upload state.</span></span> <span data-ttu-id="4a068-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4a068-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4a068-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4a068-189">publishingState</span></span>|[<span data-ttu-id="4a068-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4a068-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4a068-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a068-191">The publishing state for the app.</span></span> <span data-ttu-id="4a068-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4a068-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4a068-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4a068-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4a068-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4a068-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4a068-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4a068-195">isAssigned</span></span>|<span data-ttu-id="4a068-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a068-196">Boolean</span></span>|<span data-ttu-id="4a068-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4a068-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4a068-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4a068-199">roleScopeTagIds</span></span>|<span data-ttu-id="4a068-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a068-200">String collection</span></span>|<span data-ttu-id="4a068-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4a068-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4a068-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4a068-203">dependentAppCount</span></span>|<span data-ttu-id="4a068-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4a068-204">Int32</span></span>|<span data-ttu-id="4a068-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="4a068-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4a068-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4a068-207">supersedingAppCount</span></span>|<span data-ttu-id="4a068-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4a068-208">Int32</span></span>|<span data-ttu-id="4a068-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="4a068-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4a068-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4a068-211">supersededAppCount</span></span>|<span data-ttu-id="4a068-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4a068-212">Int32</span></span>|<span data-ttu-id="4a068-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="4a068-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4a068-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4a068-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4a068-215">committedContentVersion</span></span>|<span data-ttu-id="4a068-216">String</span><span class="sxs-lookup"><span data-stu-id="4a068-216">String</span></span>|<span data-ttu-id="4a068-217">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="4a068-217">The internal committed content version.</span></span> <span data-ttu-id="4a068-218">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4a068-219">fileName</span><span class="sxs-lookup"><span data-stu-id="4a068-219">fileName</span></span>|<span data-ttu-id="4a068-220">String</span><span class="sxs-lookup"><span data-stu-id="4a068-220">String</span></span>|<span data-ttu-id="4a068-221">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="4a068-221">The name of the main Lob application file.</span></span> <span data-ttu-id="4a068-222">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4a068-223">size</span><span class="sxs-lookup"><span data-stu-id="4a068-223">size</span></span>|<span data-ttu-id="4a068-224">Int64</span><span class="sxs-lookup"><span data-stu-id="4a068-224">Int64</span></span>|<span data-ttu-id="4a068-225">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="4a068-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="4a068-226">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="4a068-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="4a068-227">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="4a068-227">applicableArchitectures</span></span>|[<span data-ttu-id="4a068-228">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4a068-228">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4a068-229">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4a068-229">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="4a068-230">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="4a068-230">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4a068-231">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="4a068-231">applicableDeviceTypes</span></span>|[<span data-ttu-id="4a068-232">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="4a068-232">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="4a068-233">Os tipos de dispositivos Windows nos quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="4a068-233">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="4a068-234">Os valores possíveis são: `none`, `desktop`, `mobile`, `holographic`, `team`.</span><span class="sxs-lookup"><span data-stu-id="4a068-234">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="4a068-235">identityName</span><span class="sxs-lookup"><span data-stu-id="4a068-235">identityName</span></span>|<span data-ttu-id="4a068-236">String</span><span class="sxs-lookup"><span data-stu-id="4a068-236">String</span></span>|<span data-ttu-id="4a068-237">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-237">The Identity Name.</span></span>|
|<span data-ttu-id="4a068-238">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="4a068-238">identityPublisherHash</span></span>|<span data-ttu-id="4a068-239">String</span><span class="sxs-lookup"><span data-stu-id="4a068-239">String</span></span>|<span data-ttu-id="4a068-240">O Hash do Publicador de Identidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-240">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="4a068-241">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a068-241">identityResourceIdentifier</span></span>|<span data-ttu-id="4a068-242">String</span><span class="sxs-lookup"><span data-stu-id="4a068-242">String</span></span>|<span data-ttu-id="4a068-243">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-243">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4a068-244">isBundle</span><span class="sxs-lookup"><span data-stu-id="4a068-244">isBundle</span></span>|<span data-ttu-id="4a068-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a068-245">Boolean</span></span>|<span data-ttu-id="4a068-246">Se o aplicativo é um pacote ou não.</span><span class="sxs-lookup"><span data-stu-id="4a068-246">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="4a068-247">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4a068-247">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4a068-248">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4a068-248">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4a068-249">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="4a068-249">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4a068-250">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4a068-250">identityVersion</span></span>|<span data-ttu-id="4a068-251">String</span><span class="sxs-lookup"><span data-stu-id="4a068-251">String</span></span>|<span data-ttu-id="4a068-252">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="4a068-252">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="4a068-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a068-253">Response</span></span>
<span data-ttu-id="4a068-254">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a068-254">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a068-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a068-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a068-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a068-256">Request</span></span>
<span data-ttu-id="4a068-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a068-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1564

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="4a068-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a068-258">Response</span></span>
<span data-ttu-id="4a068-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a068-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1736

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true
  },
  "identityVersion": "Identity Version value"
}
```




