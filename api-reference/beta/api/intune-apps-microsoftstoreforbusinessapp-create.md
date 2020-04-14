---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5653286d465a6c62bfe7a23383ed7384b23d51a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43405434"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="62a5a-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="62a5a-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="62a5a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62a5a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62a5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62a5a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a5a-107">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="62a5a-107">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62a5a-108">Prerequisites</span></span>
<span data-ttu-id="62a5a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62a5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62a5a-111">Permission type</span></span>|<span data-ttu-id="62a5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62a5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62a5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62a5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62a5a-116">Not supported.</span></span>|
|<span data-ttu-id="62a5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a5a-117">Application</span></span>|<span data-ttu-id="62a5a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a5a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62a5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="62a5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-120">Request headers</span></span>
|<span data-ttu-id="62a5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62a5a-121">Header</span></span>|<span data-ttu-id="62a5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="62a5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="62a5a-123">Authorization</span></span>|<span data-ttu-id="62a5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62a5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a5a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62a5a-125">Accept</span></span>|<span data-ttu-id="62a5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-127">Request body</span></span>
<span data-ttu-id="62a5a-128">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="62a5a-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="62a5a-129">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="62a5a-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="62a5a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62a5a-130">Property</span></span>|<span data-ttu-id="62a5a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="62a5a-131">Type</span></span>|<span data-ttu-id="62a5a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="62a5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a5a-133">id</span><span class="sxs-lookup"><span data-stu-id="62a5a-133">id</span></span>|<span data-ttu-id="62a5a-134">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-134">String</span></span>|<span data-ttu-id="62a5a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="62a5a-135">Key of the entity.</span></span> <span data-ttu-id="62a5a-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="62a5a-137">displayName</span></span>|<span data-ttu-id="62a5a-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62a5a-138">String</span></span>|<span data-ttu-id="62a5a-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="62a5a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="62a5a-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-141">description</span><span class="sxs-lookup"><span data-stu-id="62a5a-141">description</span></span>|<span data-ttu-id="62a5a-142">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-142">String</span></span>|<span data-ttu-id="62a5a-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-143">The description of the app.</span></span> <span data-ttu-id="62a5a-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-145">publicador</span><span class="sxs-lookup"><span data-stu-id="62a5a-145">publisher</span></span>|<span data-ttu-id="62a5a-146">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-146">String</span></span>|<span data-ttu-id="62a5a-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-147">The publisher of the app.</span></span> <span data-ttu-id="62a5a-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="62a5a-149">largeIcon</span></span>|[<span data-ttu-id="62a5a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="62a5a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="62a5a-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="62a5a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="62a5a-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62a5a-153">createdDateTime</span></span>|<span data-ttu-id="62a5a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a5a-154">DateTimeOffset</span></span>|<span data-ttu-id="62a5a-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-155">The date and time the app was created.</span></span> <span data-ttu-id="62a5a-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62a5a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="62a5a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a5a-158">DateTimeOffset</span></span>|<span data-ttu-id="62a5a-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="62a5a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="62a5a-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="62a5a-161">isFeatured</span></span>|<span data-ttu-id="62a5a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="62a5a-162">Boolean</span></span>|<span data-ttu-id="62a5a-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="62a5a-164">privacyInformationUrl</span></span>|<span data-ttu-id="62a5a-165">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-165">String</span></span>|<span data-ttu-id="62a5a-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="62a5a-166">The privacy statement Url.</span></span> <span data-ttu-id="62a5a-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="62a5a-168">informationUrl</span></span>|<span data-ttu-id="62a5a-169">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-169">String</span></span>|<span data-ttu-id="62a5a-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="62a5a-170">The more information Url.</span></span> <span data-ttu-id="62a5a-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-172">owner</span><span class="sxs-lookup"><span data-stu-id="62a5a-172">owner</span></span>|<span data-ttu-id="62a5a-173">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-173">String</span></span>|<span data-ttu-id="62a5a-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-174">The owner of the app.</span></span> <span data-ttu-id="62a5a-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-176">developer</span><span class="sxs-lookup"><span data-stu-id="62a5a-176">developer</span></span>|<span data-ttu-id="62a5a-177">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-177">String</span></span>|<span data-ttu-id="62a5a-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-178">The developer of the app.</span></span> <span data-ttu-id="62a5a-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-180">notes</span><span class="sxs-lookup"><span data-stu-id="62a5a-180">notes</span></span>|<span data-ttu-id="62a5a-181">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-181">String</span></span>|<span data-ttu-id="62a5a-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-182">Notes for the app.</span></span> <span data-ttu-id="62a5a-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="62a5a-184">uploadState</span></span>|<span data-ttu-id="62a5a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="62a5a-185">Int32</span></span>|<span data-ttu-id="62a5a-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="62a5a-186">The upload state.</span></span> <span data-ttu-id="62a5a-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="62a5a-188">publishingState</span></span>|[<span data-ttu-id="62a5a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="62a5a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="62a5a-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-190">The publishing state for the app.</span></span> <span data-ttu-id="62a5a-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="62a5a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="62a5a-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="62a5a-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="62a5a-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="62a5a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="62a5a-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="62a5a-194">isAssigned</span></span>|<span data-ttu-id="62a5a-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="62a5a-195">Boolean</span></span>|<span data-ttu-id="62a5a-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="62a5a-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62a5a-198">roleScopeTagIds</span></span>|<span data-ttu-id="62a5a-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="62a5a-199">String collection</span></span>|<span data-ttu-id="62a5a-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="62a5a-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="62a5a-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="62a5a-202">dependentAppCount</span></span>|<span data-ttu-id="62a5a-203">Int32</span><span class="sxs-lookup"><span data-stu-id="62a5a-203">Int32</span></span>|<span data-ttu-id="62a5a-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="62a5a-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="62a5a-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="62a5a-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="62a5a-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62a5a-206">usedLicenseCount</span></span>|<span data-ttu-id="62a5a-207">Int32</span><span class="sxs-lookup"><span data-stu-id="62a5a-207">Int32</span></span>|<span data-ttu-id="62a5a-208">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="62a5a-208">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="62a5a-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="62a5a-209">totalLicenseCount</span></span>|<span data-ttu-id="62a5a-210">Int32</span><span class="sxs-lookup"><span data-stu-id="62a5a-210">Int32</span></span>|<span data-ttu-id="62a5a-211">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="62a5a-211">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="62a5a-212">productKey</span><span class="sxs-lookup"><span data-stu-id="62a5a-212">productKey</span></span>|<span data-ttu-id="62a5a-213">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-213">String</span></span>|<span data-ttu-id="62a5a-214">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a5a-214">The app product key</span></span>|
|<span data-ttu-id="62a5a-215">licenseType</span><span class="sxs-lookup"><span data-stu-id="62a5a-215">licenseType</span></span>|[<span data-ttu-id="62a5a-216">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="62a5a-216">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="62a5a-217">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62a5a-217">The app license type.</span></span> <span data-ttu-id="62a5a-218">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="62a5a-218">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="62a5a-219">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="62a5a-219">packageIdentityName</span></span>|<span data-ttu-id="62a5a-220">String</span><span class="sxs-lookup"><span data-stu-id="62a5a-220">String</span></span>|<span data-ttu-id="62a5a-221">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="62a5a-221">The app package identifier</span></span>|
|<span data-ttu-id="62a5a-222">licensingType</span><span class="sxs-lookup"><span data-stu-id="62a5a-222">licensingType</span></span>|[<span data-ttu-id="62a5a-223">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="62a5a-223">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="62a5a-224">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="62a5a-224">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="62a5a-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a5a-225">Response</span></span>
<span data-ttu-id="62a5a-226">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62a5a-226">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a5a-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62a5a-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a5a-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62a5a-228">Request</span></span>
<span data-ttu-id="62a5a-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62a5a-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1132

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

### <a name="response"></a><span data-ttu-id="62a5a-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="62a5a-230">Response</span></span>
<span data-ttu-id="62a5a-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62a5a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1304

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



