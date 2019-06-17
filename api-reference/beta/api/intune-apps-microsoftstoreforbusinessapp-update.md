---
title: Atualizar microsoftStoreForBusinessApp
description: Atualiza as propriedades de um objeto microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f37ede347f2d35186305a0d9c04bed4651ace2e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974367"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="546e2-103">Atualizar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="546e2-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="546e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="546e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="546e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="546e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="546e2-106">Atualiza as propriedades de um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="546e2-106">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="546e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="546e2-107">Prerequisites</span></span>
<span data-ttu-id="546e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="546e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="546e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="546e2-110">Permission type</span></span>|<span data-ttu-id="546e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="546e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="546e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="546e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="546e2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="546e2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="546e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="546e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="546e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="546e2-115">Not supported.</span></span>|
|<span data-ttu-id="546e2-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="546e2-116">Application</span></span>|<span data-ttu-id="546e2-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="546e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="546e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="546e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="546e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="546e2-119">Request headers</span></span>
|<span data-ttu-id="546e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="546e2-120">Header</span></span>|<span data-ttu-id="546e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="546e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="546e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="546e2-122">Authorization</span></span>|<span data-ttu-id="546e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="546e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="546e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="546e2-124">Accept</span></span>|<span data-ttu-id="546e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="546e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="546e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="546e2-126">Request body</span></span>
<span data-ttu-id="546e2-127">No corpo da solicitação, forneça uma representação JSON do objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="546e2-127">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="546e2-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="546e2-128">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="546e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="546e2-129">Property</span></span>|<span data-ttu-id="546e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="546e2-130">Type</span></span>|<span data-ttu-id="546e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="546e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="546e2-132">id</span><span class="sxs-lookup"><span data-stu-id="546e2-132">id</span></span>|<span data-ttu-id="546e2-133">String</span><span class="sxs-lookup"><span data-stu-id="546e2-133">String</span></span>|<span data-ttu-id="546e2-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="546e2-134">Key of the entity.</span></span> <span data-ttu-id="546e2-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="546e2-136">displayName</span></span>|<span data-ttu-id="546e2-137">String</span><span class="sxs-lookup"><span data-stu-id="546e2-137">String</span></span>|<span data-ttu-id="546e2-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="546e2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="546e2-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-140">descrição</span><span class="sxs-lookup"><span data-stu-id="546e2-140">description</span></span>|<span data-ttu-id="546e2-141">String</span><span class="sxs-lookup"><span data-stu-id="546e2-141">String</span></span>|<span data-ttu-id="546e2-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-142">The description of the app.</span></span> <span data-ttu-id="546e2-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-144">publicador</span><span class="sxs-lookup"><span data-stu-id="546e2-144">publisher</span></span>|<span data-ttu-id="546e2-145">String</span><span class="sxs-lookup"><span data-stu-id="546e2-145">String</span></span>|<span data-ttu-id="546e2-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-146">The publisher of the app.</span></span> <span data-ttu-id="546e2-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="546e2-148">largeIcon</span></span>|[<span data-ttu-id="546e2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="546e2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="546e2-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="546e2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="546e2-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="546e2-152">createdDateTime</span></span>|<span data-ttu-id="546e2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546e2-153">DateTimeOffset</span></span>|<span data-ttu-id="546e2-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-154">The date and time the app was created.</span></span> <span data-ttu-id="546e2-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="546e2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="546e2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="546e2-157">DateTimeOffset</span></span>|<span data-ttu-id="546e2-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="546e2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="546e2-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="546e2-160">isFeatured</span></span>|<span data-ttu-id="546e2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="546e2-161">Boolean</span></span>|<span data-ttu-id="546e2-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="546e2-163">privacyInformationUrl</span></span>|<span data-ttu-id="546e2-164">String</span><span class="sxs-lookup"><span data-stu-id="546e2-164">String</span></span>|<span data-ttu-id="546e2-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="546e2-165">The privacy statement Url.</span></span> <span data-ttu-id="546e2-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="546e2-167">informationUrl</span></span>|<span data-ttu-id="546e2-168">String</span><span class="sxs-lookup"><span data-stu-id="546e2-168">String</span></span>|<span data-ttu-id="546e2-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="546e2-169">The more information Url.</span></span> <span data-ttu-id="546e2-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-171">owner</span><span class="sxs-lookup"><span data-stu-id="546e2-171">owner</span></span>|<span data-ttu-id="546e2-172">String</span><span class="sxs-lookup"><span data-stu-id="546e2-172">String</span></span>|<span data-ttu-id="546e2-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="546e2-173">The owner of the app.</span></span> <span data-ttu-id="546e2-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-175">developer</span><span class="sxs-lookup"><span data-stu-id="546e2-175">developer</span></span>|<span data-ttu-id="546e2-176">String</span><span class="sxs-lookup"><span data-stu-id="546e2-176">String</span></span>|<span data-ttu-id="546e2-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-177">The developer of the app.</span></span> <span data-ttu-id="546e2-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-179">notes</span><span class="sxs-lookup"><span data-stu-id="546e2-179">notes</span></span>|<span data-ttu-id="546e2-180">String</span><span class="sxs-lookup"><span data-stu-id="546e2-180">String</span></span>|<span data-ttu-id="546e2-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-181">Notes for the app.</span></span> <span data-ttu-id="546e2-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="546e2-183">uploadState</span></span>|<span data-ttu-id="546e2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="546e2-184">Int32</span></span>|<span data-ttu-id="546e2-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="546e2-185">The upload state.</span></span> <span data-ttu-id="546e2-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="546e2-187">publishingState</span></span>|[<span data-ttu-id="546e2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="546e2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="546e2-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-189">The publishing state for the app.</span></span> <span data-ttu-id="546e2-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="546e2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="546e2-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="546e2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="546e2-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="546e2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="546e2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="546e2-193">isAssigned</span></span>|<span data-ttu-id="546e2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="546e2-194">Boolean</span></span>|<span data-ttu-id="546e2-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="546e2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="546e2-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="546e2-197">roleScopeTagIds</span></span>|<span data-ttu-id="546e2-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="546e2-198">String collection</span></span>|<span data-ttu-id="546e2-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="546e2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="546e2-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="546e2-201">dependentAppCount</span></span>|<span data-ttu-id="546e2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="546e2-202">Int32</span></span>|<span data-ttu-id="546e2-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="546e2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="546e2-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="546e2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="546e2-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="546e2-205">usedLicenseCount</span></span>|<span data-ttu-id="546e2-206">Int32</span><span class="sxs-lookup"><span data-stu-id="546e2-206">Int32</span></span>|<span data-ttu-id="546e2-207">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="546e2-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="546e2-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="546e2-208">totalLicenseCount</span></span>|<span data-ttu-id="546e2-209">Int32</span><span class="sxs-lookup"><span data-stu-id="546e2-209">Int32</span></span>|<span data-ttu-id="546e2-210">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="546e2-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="546e2-211">productKey</span><span class="sxs-lookup"><span data-stu-id="546e2-211">productKey</span></span>|<span data-ttu-id="546e2-212">String</span><span class="sxs-lookup"><span data-stu-id="546e2-212">String</span></span>|<span data-ttu-id="546e2-213">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="546e2-213">The app product key</span></span>|
|<span data-ttu-id="546e2-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="546e2-214">licenseType</span></span>|[<span data-ttu-id="546e2-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="546e2-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="546e2-216">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="546e2-216">The app license type.</span></span> <span data-ttu-id="546e2-217">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="546e2-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="546e2-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="546e2-218">packageIdentityName</span></span>|<span data-ttu-id="546e2-219">String</span><span class="sxs-lookup"><span data-stu-id="546e2-219">String</span></span>|<span data-ttu-id="546e2-220">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="546e2-220">The app package identifier</span></span>|
|<span data-ttu-id="546e2-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="546e2-221">licensingType</span></span>|[<span data-ttu-id="546e2-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="546e2-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="546e2-223">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="546e2-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="546e2-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="546e2-224">Response</span></span>
<span data-ttu-id="546e2-225">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="546e2-225">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="546e2-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="546e2-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="546e2-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="546e2-227">Request</span></span>
<span data-ttu-id="546e2-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="546e2-228">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="546e2-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="546e2-229">Response</span></span>
<span data-ttu-id="546e2-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="546e2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





