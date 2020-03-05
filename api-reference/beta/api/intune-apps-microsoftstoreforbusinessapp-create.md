---
title: Criar microsoftStoreForBusinessApp
description: Cria um novo objeto microsoftStoreForBusinessApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 659e4da402e992add2f8a74c89ef188df297f56d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445047"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="84979-103">Criar microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="84979-103">Create microsoftStoreForBusinessApp</span></span>

<span data-ttu-id="84979-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84979-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84979-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84979-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84979-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84979-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84979-107">Cria um novo objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="84979-107">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84979-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84979-108">Prerequisites</span></span>
<span data-ttu-id="84979-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84979-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84979-111">Permission type</span></span>|<span data-ttu-id="84979-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84979-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84979-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84979-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84979-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84979-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="84979-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84979-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84979-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84979-116">Not supported.</span></span>|
|<span data-ttu-id="84979-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84979-117">Application</span></span>|<span data-ttu-id="84979-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84979-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84979-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84979-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="84979-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84979-120">Request headers</span></span>
|<span data-ttu-id="84979-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84979-121">Header</span></span>|<span data-ttu-id="84979-122">Valor</span><span class="sxs-lookup"><span data-stu-id="84979-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84979-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="84979-123">Authorization</span></span>|<span data-ttu-id="84979-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84979-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84979-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84979-125">Accept</span></span>|<span data-ttu-id="84979-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84979-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84979-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84979-127">Request body</span></span>
<span data-ttu-id="84979-128">No corpo da solicitação, forneça uma representação JSON do objeto microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="84979-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="84979-129">A tabela a seguir mostra as propriedades obrigatórias ao criar microsoftStoreForBusinessApp.</span><span class="sxs-lookup"><span data-stu-id="84979-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="84979-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84979-130">Property</span></span>|<span data-ttu-id="84979-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="84979-131">Type</span></span>|<span data-ttu-id="84979-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="84979-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84979-133">id</span><span class="sxs-lookup"><span data-stu-id="84979-133">id</span></span>|<span data-ttu-id="84979-134">String</span><span class="sxs-lookup"><span data-stu-id="84979-134">String</span></span>|<span data-ttu-id="84979-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84979-135">Key of the entity.</span></span> <span data-ttu-id="84979-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-137">displayName</span><span class="sxs-lookup"><span data-stu-id="84979-137">displayName</span></span>|<span data-ttu-id="84979-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84979-138">String</span></span>|<span data-ttu-id="84979-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="84979-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="84979-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-141">description</span><span class="sxs-lookup"><span data-stu-id="84979-141">description</span></span>|<span data-ttu-id="84979-142">String</span><span class="sxs-lookup"><span data-stu-id="84979-142">String</span></span>|<span data-ttu-id="84979-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-143">The description of the app.</span></span> <span data-ttu-id="84979-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-145">publicador</span><span class="sxs-lookup"><span data-stu-id="84979-145">publisher</span></span>|<span data-ttu-id="84979-146">String</span><span class="sxs-lookup"><span data-stu-id="84979-146">String</span></span>|<span data-ttu-id="84979-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-147">The publisher of the app.</span></span> <span data-ttu-id="84979-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="84979-149">largeIcon</span></span>|[<span data-ttu-id="84979-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="84979-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="84979-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="84979-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="84979-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84979-153">createdDateTime</span></span>|<span data-ttu-id="84979-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84979-154">DateTimeOffset</span></span>|<span data-ttu-id="84979-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-155">The date and time the app was created.</span></span> <span data-ttu-id="84979-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84979-157">lastModifiedDateTime</span></span>|<span data-ttu-id="84979-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84979-158">DateTimeOffset</span></span>|<span data-ttu-id="84979-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="84979-159">The date and time the app was last modified.</span></span> <span data-ttu-id="84979-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="84979-161">isFeatured</span></span>|<span data-ttu-id="84979-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="84979-162">Boolean</span></span>|<span data-ttu-id="84979-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="84979-164">privacyInformationUrl</span></span>|<span data-ttu-id="84979-165">String</span><span class="sxs-lookup"><span data-stu-id="84979-165">String</span></span>|<span data-ttu-id="84979-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="84979-166">The privacy statement Url.</span></span> <span data-ttu-id="84979-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="84979-168">informationUrl</span></span>|<span data-ttu-id="84979-169">String</span><span class="sxs-lookup"><span data-stu-id="84979-169">String</span></span>|<span data-ttu-id="84979-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="84979-170">The more information Url.</span></span> <span data-ttu-id="84979-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-172">owner</span><span class="sxs-lookup"><span data-stu-id="84979-172">owner</span></span>|<span data-ttu-id="84979-173">String</span><span class="sxs-lookup"><span data-stu-id="84979-173">String</span></span>|<span data-ttu-id="84979-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="84979-174">The owner of the app.</span></span> <span data-ttu-id="84979-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-176">developer</span><span class="sxs-lookup"><span data-stu-id="84979-176">developer</span></span>|<span data-ttu-id="84979-177">String</span><span class="sxs-lookup"><span data-stu-id="84979-177">String</span></span>|<span data-ttu-id="84979-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-178">The developer of the app.</span></span> <span data-ttu-id="84979-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-180">notes</span><span class="sxs-lookup"><span data-stu-id="84979-180">notes</span></span>|<span data-ttu-id="84979-181">String</span><span class="sxs-lookup"><span data-stu-id="84979-181">String</span></span>|<span data-ttu-id="84979-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-182">Notes for the app.</span></span> <span data-ttu-id="84979-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="84979-184">uploadState</span></span>|<span data-ttu-id="84979-185">Int32</span><span class="sxs-lookup"><span data-stu-id="84979-185">Int32</span></span>|<span data-ttu-id="84979-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="84979-186">The upload state.</span></span> <span data-ttu-id="84979-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="84979-188">publishingState</span></span>|[<span data-ttu-id="84979-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="84979-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="84979-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-190">The publishing state for the app.</span></span> <span data-ttu-id="84979-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="84979-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="84979-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="84979-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="84979-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="84979-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="84979-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="84979-194">isAssigned</span></span>|<span data-ttu-id="84979-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="84979-195">Boolean</span></span>|<span data-ttu-id="84979-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="84979-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="84979-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84979-198">roleScopeTagIds</span></span>|<span data-ttu-id="84979-199">String collection</span><span class="sxs-lookup"><span data-stu-id="84979-199">String collection</span></span>|<span data-ttu-id="84979-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="84979-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="84979-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="84979-202">dependentAppCount</span></span>|<span data-ttu-id="84979-203">Int32</span><span class="sxs-lookup"><span data-stu-id="84979-203">Int32</span></span>|<span data-ttu-id="84979-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="84979-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="84979-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="84979-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="84979-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="84979-206">usedLicenseCount</span></span>|<span data-ttu-id="84979-207">Int32</span><span class="sxs-lookup"><span data-stu-id="84979-207">Int32</span></span>|<span data-ttu-id="84979-208">O número de aplicativos da Microsoft Store for Business em uso.</span><span class="sxs-lookup"><span data-stu-id="84979-208">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="84979-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="84979-209">totalLicenseCount</span></span>|<span data-ttu-id="84979-210">Int32</span><span class="sxs-lookup"><span data-stu-id="84979-210">Int32</span></span>|<span data-ttu-id="84979-211">O número total de aplicativos da Microsoft Store for Business.</span><span class="sxs-lookup"><span data-stu-id="84979-211">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="84979-212">productKey</span><span class="sxs-lookup"><span data-stu-id="84979-212">productKey</span></span>|<span data-ttu-id="84979-213">String</span><span class="sxs-lookup"><span data-stu-id="84979-213">String</span></span>|<span data-ttu-id="84979-214">A chave de produto do aplicativo</span><span class="sxs-lookup"><span data-stu-id="84979-214">The app product key</span></span>|
|<span data-ttu-id="84979-215">licenseType</span><span class="sxs-lookup"><span data-stu-id="84979-215">licenseType</span></span>|[<span data-ttu-id="84979-216">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="84979-216">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="84979-217">O tipo de licença do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="84979-217">The app license type.</span></span> <span data-ttu-id="84979-218">Os valores possíveis são: `offline` e `online`.</span><span class="sxs-lookup"><span data-stu-id="84979-218">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="84979-219">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="84979-219">packageIdentityName</span></span>|<span data-ttu-id="84979-220">String</span><span class="sxs-lookup"><span data-stu-id="84979-220">String</span></span>|<span data-ttu-id="84979-221">O identificador do pacote do aplicativo</span><span class="sxs-lookup"><span data-stu-id="84979-221">The app package identifier</span></span>|
|<span data-ttu-id="84979-222">licensingType</span><span class="sxs-lookup"><span data-stu-id="84979-222">licensingType</span></span>|[<span data-ttu-id="84979-223">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="84979-223">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="84979-224">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="84979-224">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="84979-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="84979-225">Response</span></span>
<span data-ttu-id="84979-226">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84979-226">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84979-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84979-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="84979-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84979-228">Request</span></span>
<span data-ttu-id="84979-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84979-229">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="84979-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="84979-230">Response</span></span>
<span data-ttu-id="84979-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84979-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





