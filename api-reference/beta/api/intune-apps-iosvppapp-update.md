---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 48c81fc18f005b4418164035b27be6093e968692
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173553"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="ff732-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="ff732-103">Update iosVppApp</span></span>

> <span data-ttu-id="ff732-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff732-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff732-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff732-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff732-106">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff732-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff732-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff732-107">Prerequisites</span></span>
<span data-ttu-id="ff732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff732-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff732-110">Permission type</span></span>|<span data-ttu-id="ff732-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff732-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff732-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff732-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff732-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff732-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff732-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff732-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff732-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff732-115">Not supported.</span></span>|
|<span data-ttu-id="ff732-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff732-116">Application</span></span>|<span data-ttu-id="ff732-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff732-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff732-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff732-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ff732-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff732-119">Request headers</span></span>
|<span data-ttu-id="ff732-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff732-120">Header</span></span>|<span data-ttu-id="ff732-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff732-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff732-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff732-122">Authorization</span></span>|<span data-ttu-id="ff732-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff732-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff732-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff732-124">Accept</span></span>|<span data-ttu-id="ff732-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff732-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff732-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff732-126">Request body</span></span>
<span data-ttu-id="ff732-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff732-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="ff732-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff732-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="ff732-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff732-129">Property</span></span>|<span data-ttu-id="ff732-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff732-130">Type</span></span>|<span data-ttu-id="ff732-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff732-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff732-132">id</span><span class="sxs-lookup"><span data-stu-id="ff732-132">id</span></span>|<span data-ttu-id="ff732-133">String</span><span class="sxs-lookup"><span data-stu-id="ff732-133">String</span></span>|<span data-ttu-id="ff732-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ff732-134">Key of the entity.</span></span> <span data-ttu-id="ff732-135">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ff732-136">displayName</span></span>|<span data-ttu-id="ff732-137">String</span><span class="sxs-lookup"><span data-stu-id="ff732-137">String</span></span>|<span data-ttu-id="ff732-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="ff732-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff732-139">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-140">descrição</span><span class="sxs-lookup"><span data-stu-id="ff732-140">description</span></span>|<span data-ttu-id="ff732-141">String</span><span class="sxs-lookup"><span data-stu-id="ff732-141">String</span></span>|<span data-ttu-id="ff732-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-142">The description of the app.</span></span> <span data-ttu-id="ff732-143">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-144">publicador</span><span class="sxs-lookup"><span data-stu-id="ff732-144">publisher</span></span>|<span data-ttu-id="ff732-145">String</span><span class="sxs-lookup"><span data-stu-id="ff732-145">String</span></span>|<span data-ttu-id="ff732-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-146">The publisher of the app.</span></span> <span data-ttu-id="ff732-147">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff732-148">largeIcon</span></span>|[<span data-ttu-id="ff732-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff732-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff732-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="ff732-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff732-151">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff732-152">createdDateTime</span></span>|<span data-ttu-id="ff732-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff732-153">DateTimeOffset</span></span>|<span data-ttu-id="ff732-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-154">The date and time the app was created.</span></span> <span data-ttu-id="ff732-155">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff732-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ff732-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff732-157">DateTimeOffset</span></span>|<span data-ttu-id="ff732-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ff732-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ff732-159">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff732-160">isFeatured</span></span>|<span data-ttu-id="ff732-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff732-161">Boolean</span></span>|<span data-ttu-id="ff732-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff732-163">privacyInformationUrl</span></span>|<span data-ttu-id="ff732-164">String</span><span class="sxs-lookup"><span data-stu-id="ff732-164">String</span></span>|<span data-ttu-id="ff732-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="ff732-165">The privacy statement Url.</span></span> <span data-ttu-id="ff732-166">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff732-167">informationUrl</span></span>|<span data-ttu-id="ff732-168">String</span><span class="sxs-lookup"><span data-stu-id="ff732-168">String</span></span>|<span data-ttu-id="ff732-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ff732-169">The more information Url.</span></span> <span data-ttu-id="ff732-170">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-171">owner</span><span class="sxs-lookup"><span data-stu-id="ff732-171">owner</span></span>|<span data-ttu-id="ff732-172">String</span><span class="sxs-lookup"><span data-stu-id="ff732-172">String</span></span>|<span data-ttu-id="ff732-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="ff732-173">The owner of the app.</span></span> <span data-ttu-id="ff732-174">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-175">developer</span><span class="sxs-lookup"><span data-stu-id="ff732-175">developer</span></span>|<span data-ttu-id="ff732-176">String</span><span class="sxs-lookup"><span data-stu-id="ff732-176">String</span></span>|<span data-ttu-id="ff732-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-177">The developer of the app.</span></span> <span data-ttu-id="ff732-178">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-179">notes</span><span class="sxs-lookup"><span data-stu-id="ff732-179">notes</span></span>|<span data-ttu-id="ff732-180">String</span><span class="sxs-lookup"><span data-stu-id="ff732-180">String</span></span>|<span data-ttu-id="ff732-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-181">Notes for the app.</span></span> <span data-ttu-id="ff732-182">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="ff732-183">uploadState</span></span>|<span data-ttu-id="ff732-184">Int32</span><span class="sxs-lookup"><span data-stu-id="ff732-184">Int32</span></span>|<span data-ttu-id="ff732-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="ff732-185">The upload state.</span></span> <span data-ttu-id="ff732-186">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff732-187">publishingState</span></span>|[<span data-ttu-id="ff732-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ff732-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff732-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-189">The publishing state for the app.</span></span> <span data-ttu-id="ff732-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="ff732-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff732-191">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="ff732-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ff732-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="ff732-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff732-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff732-193">isAssigned</span></span>|<span data-ttu-id="ff732-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff732-194">Boolean</span></span>|<span data-ttu-id="ff732-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="ff732-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ff732-196">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff732-197">roleScopeTagIds</span></span>|<span data-ttu-id="ff732-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff732-198">String collection</span></span>|<span data-ttu-id="ff732-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="ff732-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ff732-200">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ff732-201">dependentAppCount</span></span>|<span data-ttu-id="ff732-202">Int32</span><span class="sxs-lookup"><span data-stu-id="ff732-202">Int32</span></span>|<span data-ttu-id="ff732-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="ff732-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ff732-204">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff732-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff732-205">usedLicenseCount</span></span>|<span data-ttu-id="ff732-206">Int32</span><span class="sxs-lookup"><span data-stu-id="ff732-206">Int32</span></span>|<span data-ttu-id="ff732-207">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="ff732-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="ff732-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff732-208">totalLicenseCount</span></span>|<span data-ttu-id="ff732-209">Int32</span><span class="sxs-lookup"><span data-stu-id="ff732-209">Int32</span></span>|<span data-ttu-id="ff732-210">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="ff732-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="ff732-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="ff732-211">releaseDateTime</span></span>|<span data-ttu-id="ff732-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff732-212">DateTimeOffset</span></span>|<span data-ttu-id="ff732-213">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="ff732-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="ff732-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="ff732-214">appStoreUrl</span></span>|<span data-ttu-id="ff732-215">String</span><span class="sxs-lookup"><span data-stu-id="ff732-215">String</span></span>|<span data-ttu-id="ff732-216">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="ff732-216">The store URL.</span></span>|
|<span data-ttu-id="ff732-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="ff732-217">licensingType</span></span>|[<span data-ttu-id="ff732-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="ff732-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="ff732-219">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="ff732-219">The supported License Type.</span></span>|
|<span data-ttu-id="ff732-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ff732-220">applicableDeviceType</span></span>|[<span data-ttu-id="ff732-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ff732-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ff732-222">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="ff732-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="ff732-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ff732-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="ff732-224">String</span><span class="sxs-lookup"><span data-stu-id="ff732-224">String</span></span>|<span data-ttu-id="ff732-225">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="ff732-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ff732-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ff732-226">vppTokenAccountType</span></span>|[<span data-ttu-id="ff732-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ff732-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="ff732-228">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="ff732-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ff732-229">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="ff732-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ff732-230">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="ff732-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ff732-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="ff732-231">vppTokenAppleId</span></span>|<span data-ttu-id="ff732-232">String</span><span class="sxs-lookup"><span data-stu-id="ff732-232">String</span></span>|<span data-ttu-id="ff732-233">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="ff732-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ff732-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="ff732-234">bundleId</span></span>|<span data-ttu-id="ff732-235">String</span><span class="sxs-lookup"><span data-stu-id="ff732-235">String</span></span>|<span data-ttu-id="ff732-236">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="ff732-236">The Identity Name.</span></span>|
|<span data-ttu-id="ff732-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ff732-237">vppTokenId</span></span>|<span data-ttu-id="ff732-238">String</span><span class="sxs-lookup"><span data-stu-id="ff732-238">String</span></span>|<span data-ttu-id="ff732-239">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="ff732-240">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="ff732-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="ff732-241">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="ff732-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="ff732-242">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff732-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="ff732-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff732-243">Response</span></span>
<span data-ttu-id="ff732-244">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff732-244">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff732-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff732-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff732-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff732-246">Request</span></span>
<span data-ttu-id="ff732-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff732-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1999

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ff732-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff732-248">Response</span></span>
<span data-ttu-id="ff732-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff732-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2171

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




