---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd2d57abe08687d5066b6fcf66da4cedca4cb49a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935444"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="17ca9-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="17ca9-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="17ca9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="17ca9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17ca9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="17ca9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17ca9-106">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ca9-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17ca9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="17ca9-107">Prerequisites</span></span>
<span data-ttu-id="17ca9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17ca9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17ca9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17ca9-110">Permission type</span></span>|<span data-ttu-id="17ca9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="17ca9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17ca9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17ca9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17ca9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17ca9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="17ca9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17ca9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17ca9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17ca9-115">Not supported.</span></span>|
|<span data-ttu-id="17ca9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17ca9-116">Application</span></span>|<span data-ttu-id="17ca9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17ca9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17ca9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17ca9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="17ca9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17ca9-119">Request headers</span></span>
|<span data-ttu-id="17ca9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="17ca9-120">Header</span></span>|<span data-ttu-id="17ca9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="17ca9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17ca9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="17ca9-122">Authorization</span></span>|<span data-ttu-id="17ca9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17ca9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17ca9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="17ca9-124">Accept</span></span>|<span data-ttu-id="17ca9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="17ca9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17ca9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17ca9-126">Request body</span></span>
<span data-ttu-id="17ca9-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="17ca9-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="17ca9-128">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="17ca9-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="17ca9-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17ca9-129">Property</span></span>|<span data-ttu-id="17ca9-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="17ca9-130">Type</span></span>|<span data-ttu-id="17ca9-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="17ca9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17ca9-132">id</span><span class="sxs-lookup"><span data-stu-id="17ca9-132">id</span></span>|<span data-ttu-id="17ca9-133">String</span><span class="sxs-lookup"><span data-stu-id="17ca9-133">String</span></span>|<span data-ttu-id="17ca9-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="17ca9-134">Key of the entity.</span></span> <span data-ttu-id="17ca9-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="17ca9-136">displayName</span></span>|<span data-ttu-id="17ca9-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-137">String</span></span>|<span data-ttu-id="17ca9-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="17ca9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="17ca9-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-140">description</span><span class="sxs-lookup"><span data-stu-id="17ca9-140">description</span></span>|<span data-ttu-id="17ca9-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-141">String</span></span>|<span data-ttu-id="17ca9-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-142">The description of the app.</span></span> <span data-ttu-id="17ca9-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-144">publicador</span><span class="sxs-lookup"><span data-stu-id="17ca9-144">publisher</span></span>|<span data-ttu-id="17ca9-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-145">String</span></span>|<span data-ttu-id="17ca9-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-146">The publisher of the app.</span></span> <span data-ttu-id="17ca9-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="17ca9-148">largeIcon</span></span>|[<span data-ttu-id="17ca9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="17ca9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="17ca9-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="17ca9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="17ca9-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17ca9-152">createdDateTime</span></span>|<span data-ttu-id="17ca9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ca9-153">DateTimeOffset</span></span>|<span data-ttu-id="17ca9-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-154">The date and time the app was created.</span></span> <span data-ttu-id="17ca9-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="17ca9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="17ca9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17ca9-157">DateTimeOffset</span></span>|<span data-ttu-id="17ca9-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="17ca9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="17ca9-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="17ca9-160">isFeatured</span></span>|<span data-ttu-id="17ca9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ca9-161">Boolean</span></span>|<span data-ttu-id="17ca9-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="17ca9-163">privacyInformationUrl</span></span>|<span data-ttu-id="17ca9-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-164">String</span></span>|<span data-ttu-id="17ca9-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="17ca9-165">The privacy statement Url.</span></span> <span data-ttu-id="17ca9-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="17ca9-167">informationUrl</span></span>|<span data-ttu-id="17ca9-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-168">String</span></span>|<span data-ttu-id="17ca9-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="17ca9-169">The more information Url.</span></span> <span data-ttu-id="17ca9-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-171">owner</span><span class="sxs-lookup"><span data-stu-id="17ca9-171">owner</span></span>|<span data-ttu-id="17ca9-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-172">String</span></span>|<span data-ttu-id="17ca9-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-173">The owner of the app.</span></span> <span data-ttu-id="17ca9-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-175">developer</span><span class="sxs-lookup"><span data-stu-id="17ca9-175">developer</span></span>|<span data-ttu-id="17ca9-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-176">String</span></span>|<span data-ttu-id="17ca9-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-177">The developer of the app.</span></span> <span data-ttu-id="17ca9-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-179">notes</span><span class="sxs-lookup"><span data-stu-id="17ca9-179">notes</span></span>|<span data-ttu-id="17ca9-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-180">String</span></span>|<span data-ttu-id="17ca9-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-181">Notes for the app.</span></span> <span data-ttu-id="17ca9-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="17ca9-183">uploadState</span></span>|<span data-ttu-id="17ca9-184">Int32</span><span class="sxs-lookup"><span data-stu-id="17ca9-184">Int32</span></span>|<span data-ttu-id="17ca9-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="17ca9-185">The upload state.</span></span> <span data-ttu-id="17ca9-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="17ca9-187">publishingState</span></span>|[<span data-ttu-id="17ca9-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="17ca9-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="17ca9-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-189">The publishing state for the app.</span></span> <span data-ttu-id="17ca9-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="17ca9-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="17ca9-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="17ca9-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="17ca9-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="17ca9-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="17ca9-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="17ca9-193">isAssigned</span></span>|<span data-ttu-id="17ca9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="17ca9-194">Boolean</span></span>|<span data-ttu-id="17ca9-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="17ca9-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="17ca9-197">roleScopeTagIds</span></span>|<span data-ttu-id="17ca9-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-198">String collection</span></span>|<span data-ttu-id="17ca9-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="17ca9-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="17ca9-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="17ca9-201">dependentAppCount</span></span>|<span data-ttu-id="17ca9-202">Int32</span><span class="sxs-lookup"><span data-stu-id="17ca9-202">Int32</span></span>|<span data-ttu-id="17ca9-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="17ca9-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="17ca9-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="17ca9-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="17ca9-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="17ca9-205">usedLicenseCount</span></span>|<span data-ttu-id="17ca9-206">Int32</span><span class="sxs-lookup"><span data-stu-id="17ca9-206">Int32</span></span>|<span data-ttu-id="17ca9-207">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="17ca9-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="17ca9-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="17ca9-208">totalLicenseCount</span></span>|<span data-ttu-id="17ca9-209">Int32</span><span class="sxs-lookup"><span data-stu-id="17ca9-209">Int32</span></span>|<span data-ttu-id="17ca9-210">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="17ca9-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="17ca9-211">productKey</span><span class="sxs-lookup"><span data-stu-id="17ca9-211">productKey</span></span>|<span data-ttu-id="17ca9-212">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="17ca9-212">String</span></span>|<span data-ttu-id="17ca9-213">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="17ca9-213">The app product key</span></span>|
|<span data-ttu-id="17ca9-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="17ca9-214">licenseType</span></span>|[<span data-ttu-id="17ca9-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="17ca9-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="17ca9-216">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="17ca9-216">The app license type.</span></span> <span data-ttu-id="17ca9-217">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="17ca9-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="17ca9-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="17ca9-218">packageIdentityName</span></span>|<span data-ttu-id="17ca9-219">String</span><span class="sxs-lookup"><span data-stu-id="17ca9-219">String</span></span>|<span data-ttu-id="17ca9-220">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="17ca9-220">The app package identifier</span></span>|
|<span data-ttu-id="17ca9-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="17ca9-221">licensingType</span></span>|[<span data-ttu-id="17ca9-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="17ca9-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="17ca9-223">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="17ca9-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="17ca9-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="17ca9-224">Response</span></span>
<span data-ttu-id="17ca9-225">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17ca9-225">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17ca9-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="17ca9-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="17ca9-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17ca9-227">Request</span></span>
<span data-ttu-id="17ca9-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="17ca9-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="17ca9-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="17ca9-229">Response</span></span>
<span data-ttu-id="17ca9-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="17ca9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




