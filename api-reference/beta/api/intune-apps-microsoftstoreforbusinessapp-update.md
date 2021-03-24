---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b3c10a1e094d5cde2250066da65879352a8fca9a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143434"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="4d6fd-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="4d6fd-103">Update microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="4d6fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d6fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4d6fd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d6fd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d6fd-107">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d6fd-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d6fd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d6fd-108">Prerequisites</span></span>
<span data-ttu-id="4d6fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d6fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d6fd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d6fd-111">Permission type</span></span>|<span data-ttu-id="4d6fd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d6fd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d6fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4d6fd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d6fd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-116">Not supported.</span></span>|
|<span data-ttu-id="4d6fd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d6fd-117">Application</span></span>|<span data-ttu-id="4d6fd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d6fd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d6fd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d6fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="4d6fd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6fd-120">Request headers</span></span>
|<span data-ttu-id="4d6fd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d6fd-121">Header</span></span>|<span data-ttu-id="4d6fd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d6fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d6fd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d6fd-123">Authorization</span></span>|<span data-ttu-id="4d6fd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d6fd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d6fd-125">Accept</span></span>|<span data-ttu-id="4d6fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d6fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d6fd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6fd-127">Request body</span></span>
<span data-ttu-id="4d6fd-128">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d6fd-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="4d6fd-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d6fd-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="4d6fd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d6fd-130">Property</span></span>|<span data-ttu-id="4d6fd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d6fd-131">Type</span></span>|<span data-ttu-id="4d6fd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d6fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d6fd-133">id</span><span class="sxs-lookup"><span data-stu-id="4d6fd-133">id</span></span>|<span data-ttu-id="4d6fd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d6fd-134">String</span></span>|<span data-ttu-id="4d6fd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-135">Key of the entity.</span></span> <span data-ttu-id="4d6fd-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4d6fd-137">displayName</span></span>|<span data-ttu-id="4d6fd-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d6fd-138">String</span></span>|<span data-ttu-id="4d6fd-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4d6fd-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-141">descrição</span><span class="sxs-lookup"><span data-stu-id="4d6fd-141">description</span></span>|<span data-ttu-id="4d6fd-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d6fd-142">String</span></span>|<span data-ttu-id="4d6fd-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-143">The description of the app.</span></span> <span data-ttu-id="4d6fd-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-145">publicador</span><span class="sxs-lookup"><span data-stu-id="4d6fd-145">publisher</span></span>|<span data-ttu-id="4d6fd-146">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-146">String</span></span>|<span data-ttu-id="4d6fd-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-147">The publisher of the app.</span></span> <span data-ttu-id="4d6fd-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4d6fd-149">largeIcon</span></span>|[<span data-ttu-id="4d6fd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4d6fd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4d6fd-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4d6fd-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d6fd-153">createdDateTime</span></span>|<span data-ttu-id="4d6fd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d6fd-154">DateTimeOffset</span></span>|<span data-ttu-id="4d6fd-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-155">The date and time the app was created.</span></span> <span data-ttu-id="4d6fd-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d6fd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4d6fd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d6fd-158">DateTimeOffset</span></span>|<span data-ttu-id="4d6fd-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4d6fd-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4d6fd-161">isFeatured</span></span>|<span data-ttu-id="4d6fd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d6fd-162">Boolean</span></span>|<span data-ttu-id="4d6fd-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4d6fd-164">privacyInformationUrl</span></span>|<span data-ttu-id="4d6fd-165">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-165">String</span></span>|<span data-ttu-id="4d6fd-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-166">The privacy statement Url.</span></span> <span data-ttu-id="4d6fd-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4d6fd-168">informationUrl</span></span>|<span data-ttu-id="4d6fd-169">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-169">String</span></span>|<span data-ttu-id="4d6fd-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-170">The more information Url.</span></span> <span data-ttu-id="4d6fd-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-172">owner</span><span class="sxs-lookup"><span data-stu-id="4d6fd-172">owner</span></span>|<span data-ttu-id="4d6fd-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d6fd-173">String</span></span>|<span data-ttu-id="4d6fd-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-174">The owner of the app.</span></span> <span data-ttu-id="4d6fd-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-176">developer</span><span class="sxs-lookup"><span data-stu-id="4d6fd-176">developer</span></span>|<span data-ttu-id="4d6fd-177">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-177">String</span></span>|<span data-ttu-id="4d6fd-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-178">The developer of the app.</span></span> <span data-ttu-id="4d6fd-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-180">notes</span><span class="sxs-lookup"><span data-stu-id="4d6fd-180">notes</span></span>|<span data-ttu-id="4d6fd-181">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-181">String</span></span>|<span data-ttu-id="4d6fd-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-182">Notes for the app.</span></span> <span data-ttu-id="4d6fd-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4d6fd-184">uploadState</span></span>|<span data-ttu-id="4d6fd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-185">Int32</span></span>|<span data-ttu-id="4d6fd-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-186">The upload state.</span></span> <span data-ttu-id="4d6fd-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="4d6fd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="4d6fd-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="4d6fd-189">publishingState</span></span>|[<span data-ttu-id="4d6fd-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4d6fd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4d6fd-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-191">The publishing state for the app.</span></span> <span data-ttu-id="4d6fd-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4d6fd-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="4d6fd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="4d6fd-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4d6fd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4d6fd-195">isAssigned</span></span>|<span data-ttu-id="4d6fd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d6fd-196">Boolean</span></span>|<span data-ttu-id="4d6fd-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4d6fd-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4d6fd-199">roleScopeTagIds</span></span>|<span data-ttu-id="4d6fd-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d6fd-200">String collection</span></span>|<span data-ttu-id="4d6fd-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4d6fd-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4d6fd-203">dependentAppCount</span></span>|<span data-ttu-id="4d6fd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-204">Int32</span></span>|<span data-ttu-id="4d6fd-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="4d6fd-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4d6fd-207">supersedingAppCount</span></span>|<span data-ttu-id="4d6fd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-208">Int32</span></span>|<span data-ttu-id="4d6fd-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="4d6fd-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4d6fd-211">supersededAppCount</span></span>|<span data-ttu-id="4d6fd-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-212">Int32</span></span>|<span data-ttu-id="4d6fd-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="4d6fd-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="4d6fd-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="4d6fd-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4d6fd-215">usedLicenseCount</span></span>|<span data-ttu-id="4d6fd-216">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-216">Int32</span></span>|<span data-ttu-id="4d6fd-217">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-217">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="4d6fd-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="4d6fd-218">totalLicenseCount</span></span>|<span data-ttu-id="4d6fd-219">Int32</span><span class="sxs-lookup"><span data-stu-id="4d6fd-219">Int32</span></span>|<span data-ttu-id="4d6fd-220">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-220">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="4d6fd-221">productKey</span><span class="sxs-lookup"><span data-stu-id="4d6fd-221">productKey</span></span>|<span data-ttu-id="4d6fd-222">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-222">String</span></span>|<span data-ttu-id="4d6fd-223">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d6fd-223">The app product key</span></span>|
|<span data-ttu-id="4d6fd-224">licenseType</span><span class="sxs-lookup"><span data-stu-id="4d6fd-224">licenseType</span></span>|[<span data-ttu-id="4d6fd-225">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="4d6fd-225">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="4d6fd-226">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-226">The app license type.</span></span> <span data-ttu-id="4d6fd-227">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-227">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="4d6fd-228">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="4d6fd-228">packageIdentityName</span></span>|<span data-ttu-id="4d6fd-229">String</span><span class="sxs-lookup"><span data-stu-id="4d6fd-229">String</span></span>|<span data-ttu-id="4d6fd-230">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d6fd-230">The app package identifier</span></span>|
|<span data-ttu-id="4d6fd-231">licensingType</span><span class="sxs-lookup"><span data-stu-id="4d6fd-231">licensingType</span></span>|[<span data-ttu-id="4d6fd-232">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="4d6fd-232">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="4d6fd-233">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-233">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="4d6fd-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d6fd-234">Response</span></span>
<span data-ttu-id="4d6fd-235">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-235">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d6fd-236">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d6fd-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d6fd-237">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d6fd-237">Request</span></span>
<span data-ttu-id="4d6fd-238">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="4d6fd-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d6fd-239">Response</span></span>
<span data-ttu-id="4d6fd-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d6fd-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```




