---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a58d72044986bfbc55cdcc311f7bdecdf6a2532
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336835"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="a8a8b-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="a8a8b-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="a8a8b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8a8b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8a8b-106">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8a8b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a8a8b-107">Prerequisites</span></span>
<span data-ttu-id="a8a8b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8a8b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8a8b-110">Permission type</span></span>|<span data-ttu-id="a8a8b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8a8b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8a8b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a8b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8a8b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8a8b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-115">Not supported.</span></span>|
|<span data-ttu-id="a8a8b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8a8b-116">Application</span></span>|<span data-ttu-id="a8a8b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8a8b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8a8b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8a8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a8a8b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a8b-119">Request headers</span></span>
|<span data-ttu-id="a8a8b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8a8b-120">Header</span></span>|<span data-ttu-id="a8a8b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a8a8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8a8b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8a8b-122">Authorization</span></span>|<span data-ttu-id="a8a8b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8a8b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a8a8b-124">Accept</span></span>|<span data-ttu-id="a8a8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8a8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8a8b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a8b-126">Request body</span></span>
<span data-ttu-id="a8a8b-127">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="a8a8b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="a8a8b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8a8b-129">Property</span></span>|<span data-ttu-id="a8a8b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a8b-130">Type</span></span>|<span data-ttu-id="a8a8b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a8b-132">id</span><span class="sxs-lookup"><span data-stu-id="a8a8b-132">id</span></span>|<span data-ttu-id="a8a8b-133">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-133">String</span></span>|<span data-ttu-id="a8a8b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-134">Key of the entity.</span></span> <span data-ttu-id="a8a8b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a8b-136">displayName</span></span>|<span data-ttu-id="a8a8b-137">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-137">String</span></span>|<span data-ttu-id="a8a8b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a8a8b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-140">descrição</span><span class="sxs-lookup"><span data-stu-id="a8a8b-140">description</span></span>|<span data-ttu-id="a8a8b-141">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-141">String</span></span>|<span data-ttu-id="a8a8b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-142">The description of the app.</span></span> <span data-ttu-id="a8a8b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a8a8b-144">publisher</span></span>|<span data-ttu-id="a8a8b-145">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-145">String</span></span>|<span data-ttu-id="a8a8b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-146">The publisher of the app.</span></span> <span data-ttu-id="a8a8b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a8a8b-148">largeIcon</span></span>|[<span data-ttu-id="a8a8b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a8a8b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a8a8b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a8a8b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a8b-152">createdDateTime</span></span>|<span data-ttu-id="a8a8b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a8b-153">DateTimeOffset</span></span>|<span data-ttu-id="a8a8b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-154">The date and time the app was created.</span></span> <span data-ttu-id="a8a8b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8a8b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a8a8b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8a8b-157">DateTimeOffset</span></span>|<span data-ttu-id="a8a8b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a8a8b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a8a8b-160">isFeatured</span></span>|<span data-ttu-id="a8a8b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8a8b-161">Boolean</span></span>|<span data-ttu-id="a8a8b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a8a8b-163">privacyInformationUrl</span></span>|<span data-ttu-id="a8a8b-164">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-164">String</span></span>|<span data-ttu-id="a8a8b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-165">The privacy statement Url.</span></span> <span data-ttu-id="a8a8b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a8a8b-167">informationUrl</span></span>|<span data-ttu-id="a8a8b-168">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-168">String</span></span>|<span data-ttu-id="a8a8b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-169">The more information Url.</span></span> <span data-ttu-id="a8a8b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-171">owner</span><span class="sxs-lookup"><span data-stu-id="a8a8b-171">owner</span></span>|<span data-ttu-id="a8a8b-172">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-172">String</span></span>|<span data-ttu-id="a8a8b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-173">The owner of the app.</span></span> <span data-ttu-id="a8a8b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-175">developer</span><span class="sxs-lookup"><span data-stu-id="a8a8b-175">developer</span></span>|<span data-ttu-id="a8a8b-176">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-176">String</span></span>|<span data-ttu-id="a8a8b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-177">The developer of the app.</span></span> <span data-ttu-id="a8a8b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-179">notes</span><span class="sxs-lookup"><span data-stu-id="a8a8b-179">notes</span></span>|<span data-ttu-id="a8a8b-180">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-180">String</span></span>|<span data-ttu-id="a8a8b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-181">Notes for the app.</span></span> <span data-ttu-id="a8a8b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a8a8b-183">uploadState</span></span>|<span data-ttu-id="a8a8b-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a8a8b-184">Int32</span></span>|<span data-ttu-id="a8a8b-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-185">The upload state.</span></span> <span data-ttu-id="a8a8b-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a8a8b-187">publishingState</span></span>|[<span data-ttu-id="a8a8b-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a8a8b-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a8a8b-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-189">The publishing state for the app.</span></span> <span data-ttu-id="a8a8b-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a8a8b-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a8a8b-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a8a8b-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a8a8b-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a8a8b-193">isAssigned</span></span>|<span data-ttu-id="a8a8b-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8a8b-194">Boolean</span></span>|<span data-ttu-id="a8a8b-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a8a8b-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8a8b-197">roleScopeTagIds</span></span>|<span data-ttu-id="a8a8b-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a8b-198">String collection</span></span>|<span data-ttu-id="a8a8b-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a8a8b-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a8a8b-201">dependentAppCount</span></span>|<span data-ttu-id="a8a8b-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a8a8b-202">Int32</span></span>|<span data-ttu-id="a8a8b-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a8a8b-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8a8b-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8a8b-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a8a8b-205">usedLicenseCount</span></span>|<span data-ttu-id="a8a8b-206">Int32</span><span class="sxs-lookup"><span data-stu-id="a8a8b-206">Int32</span></span>|<span data-ttu-id="a8a8b-207">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="a8a8b-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a8a8b-208">totalLicenseCount</span></span>|<span data-ttu-id="a8a8b-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a8a8b-209">Int32</span></span>|<span data-ttu-id="a8a8b-210">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="a8a8b-211">productKey</span><span class="sxs-lookup"><span data-stu-id="a8a8b-211">productKey</span></span>|<span data-ttu-id="a8a8b-212">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-212">String</span></span>|<span data-ttu-id="a8a8b-213">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8a8b-213">The app product key</span></span>|
|<span data-ttu-id="a8a8b-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="a8a8b-214">licenseType</span></span>|[<span data-ttu-id="a8a8b-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="a8a8b-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="a8a8b-216">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-216">The app license type.</span></span> <span data-ttu-id="a8a8b-217">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="a8a8b-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="a8a8b-218">packageIdentityName</span></span>|<span data-ttu-id="a8a8b-219">String</span><span class="sxs-lookup"><span data-stu-id="a8a8b-219">String</span></span>|<span data-ttu-id="a8a8b-220">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8a8b-220">The app package identifier</span></span>|
|<span data-ttu-id="a8a8b-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="a8a8b-221">licensingType</span></span>|[<span data-ttu-id="a8a8b-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a8a8b-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="a8a8b-223">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="a8a8b-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a8b-224">Response</span></span>
<span data-ttu-id="a8a8b-225">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-225">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8a8b-226">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8a8b-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8a8b-227">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8a8b-227">Request</span></span>
<span data-ttu-id="a8a8b-228">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-228">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8a8b-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8a8b-229">Response</span></span>
<span data-ttu-id="a8a8b-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a8a8b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






