---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 103902121a51683f0e74752296daf100511e2f23
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937046"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="e5527-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e5527-103">Create iosVppApp</span></span>

> <span data-ttu-id="e5527-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5527-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5527-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5527-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5527-106">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5527-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5527-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5527-107">Prerequisites</span></span>
<span data-ttu-id="e5527-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5527-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5527-110">Permission type</span></span>|<span data-ttu-id="e5527-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5527-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5527-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5527-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e5527-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5527-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e5527-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5527-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5527-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5527-115">Not supported.</span></span>|
|<span data-ttu-id="e5527-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5527-116">Application</span></span>|<span data-ttu-id="e5527-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5527-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5527-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5527-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e5527-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5527-119">Request headers</span></span>
|<span data-ttu-id="e5527-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5527-120">Header</span></span>|<span data-ttu-id="e5527-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e5527-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5527-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5527-122">Authorization</span></span>|<span data-ttu-id="e5527-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5527-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5527-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5527-124">Accept</span></span>|<span data-ttu-id="e5527-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e5527-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5527-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5527-126">Request body</span></span>
<span data-ttu-id="e5527-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="e5527-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="e5527-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="e5527-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="e5527-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5527-129">Property</span></span>|<span data-ttu-id="e5527-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5527-130">Type</span></span>|<span data-ttu-id="e5527-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5527-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5527-132">id</span><span class="sxs-lookup"><span data-stu-id="e5527-132">id</span></span>|<span data-ttu-id="e5527-133">String</span><span class="sxs-lookup"><span data-stu-id="e5527-133">String</span></span>|<span data-ttu-id="e5527-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e5527-134">Key of the entity.</span></span> <span data-ttu-id="e5527-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e5527-136">displayName</span></span>|<span data-ttu-id="e5527-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-137">String</span></span>|<span data-ttu-id="e5527-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e5527-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e5527-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-140">description</span><span class="sxs-lookup"><span data-stu-id="e5527-140">description</span></span>|<span data-ttu-id="e5527-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-141">String</span></span>|<span data-ttu-id="e5527-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-142">The description of the app.</span></span> <span data-ttu-id="e5527-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-144">publicador</span><span class="sxs-lookup"><span data-stu-id="e5527-144">publisher</span></span>|<span data-ttu-id="e5527-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-145">String</span></span>|<span data-ttu-id="e5527-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-146">The publisher of the app.</span></span> <span data-ttu-id="e5527-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e5527-148">largeIcon</span></span>|[<span data-ttu-id="e5527-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e5527-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e5527-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e5527-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e5527-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5527-152">createdDateTime</span></span>|<span data-ttu-id="e5527-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5527-153">DateTimeOffset</span></span>|<span data-ttu-id="e5527-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-154">The date and time the app was created.</span></span> <span data-ttu-id="e5527-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5527-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e5527-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5527-157">DateTimeOffset</span></span>|<span data-ttu-id="e5527-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e5527-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e5527-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e5527-160">isFeatured</span></span>|<span data-ttu-id="e5527-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5527-161">Boolean</span></span>|<span data-ttu-id="e5527-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e5527-163">privacyInformationUrl</span></span>|<span data-ttu-id="e5527-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-164">String</span></span>|<span data-ttu-id="e5527-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e5527-165">The privacy statement Url.</span></span> <span data-ttu-id="e5527-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e5527-167">informationUrl</span></span>|<span data-ttu-id="e5527-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-168">String</span></span>|<span data-ttu-id="e5527-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e5527-169">The more information Url.</span></span> <span data-ttu-id="e5527-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-171">owner</span><span class="sxs-lookup"><span data-stu-id="e5527-171">owner</span></span>|<span data-ttu-id="e5527-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-172">String</span></span>|<span data-ttu-id="e5527-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e5527-173">The owner of the app.</span></span> <span data-ttu-id="e5527-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-175">developer</span><span class="sxs-lookup"><span data-stu-id="e5527-175">developer</span></span>|<span data-ttu-id="e5527-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-176">String</span></span>|<span data-ttu-id="e5527-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-177">The developer of the app.</span></span> <span data-ttu-id="e5527-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-179">notes</span><span class="sxs-lookup"><span data-stu-id="e5527-179">notes</span></span>|<span data-ttu-id="e5527-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-180">String</span></span>|<span data-ttu-id="e5527-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-181">Notes for the app.</span></span> <span data-ttu-id="e5527-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e5527-183">uploadState</span></span>|<span data-ttu-id="e5527-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e5527-184">Int32</span></span>|<span data-ttu-id="e5527-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e5527-185">The upload state.</span></span> <span data-ttu-id="e5527-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e5527-187">publishingState</span></span>|[<span data-ttu-id="e5527-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e5527-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e5527-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-189">The publishing state for the app.</span></span> <span data-ttu-id="e5527-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e5527-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e5527-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e5527-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e5527-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e5527-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e5527-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e5527-193">isAssigned</span></span>|<span data-ttu-id="e5527-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5527-194">Boolean</span></span>|<span data-ttu-id="e5527-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e5527-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e5527-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5527-197">roleScopeTagIds</span></span>|<span data-ttu-id="e5527-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-198">String collection</span></span>|<span data-ttu-id="e5527-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e5527-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e5527-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e5527-201">dependentAppCount</span></span>|<span data-ttu-id="e5527-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e5527-202">Int32</span></span>|<span data-ttu-id="e5527-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e5527-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e5527-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e5527-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5527-205">usedLicenseCount</span></span>|<span data-ttu-id="e5527-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e5527-206">Int32</span></span>|<span data-ttu-id="e5527-207">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="e5527-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="e5527-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e5527-208">totalLicenseCount</span></span>|<span data-ttu-id="e5527-209">Int32</span><span class="sxs-lookup"><span data-stu-id="e5527-209">Int32</span></span>|<span data-ttu-id="e5527-210">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="e5527-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="e5527-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="e5527-211">releaseDateTime</span></span>|<span data-ttu-id="e5527-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5527-212">DateTimeOffset</span></span>|<span data-ttu-id="e5527-213">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="e5527-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="e5527-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e5527-214">appStoreUrl</span></span>|<span data-ttu-id="e5527-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-215">String</span></span>|<span data-ttu-id="e5527-216">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="e5527-216">The store URL.</span></span>|
|<span data-ttu-id="e5527-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="e5527-217">licensingType</span></span>|[<span data-ttu-id="e5527-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e5527-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="e5527-219">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="e5527-219">The supported License Type.</span></span>|
|<span data-ttu-id="e5527-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5527-220">applicableDeviceType</span></span>|[<span data-ttu-id="e5527-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e5527-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e5527-222">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="e5527-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="e5527-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e5527-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="e5527-224">String</span><span class="sxs-lookup"><span data-stu-id="e5527-224">String</span></span>|<span data-ttu-id="e5527-225">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="e5527-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="e5527-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e5527-226">vppTokenAccountType</span></span>|[<span data-ttu-id="e5527-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e5527-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="e5527-228">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="e5527-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="e5527-229">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="e5527-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="e5527-230">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="e5527-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="e5527-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="e5527-231">vppTokenAppleId</span></span>|<span data-ttu-id="e5527-232">String</span><span class="sxs-lookup"><span data-stu-id="e5527-232">String</span></span>|<span data-ttu-id="e5527-233">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="e5527-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="e5527-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="e5527-234">bundleId</span></span>|<span data-ttu-id="e5527-235">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-235">String</span></span>|<span data-ttu-id="e5527-236">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e5527-236">The Identity Name.</span></span>|
|<span data-ttu-id="e5527-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e5527-237">vppTokenId</span></span>|<span data-ttu-id="e5527-238">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5527-238">String</span></span>|<span data-ttu-id="e5527-239">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="e5527-240">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="e5527-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="e5527-241">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e5527-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="e5527-242">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e5527-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="e5527-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5527-243">Response</span></span>
<span data-ttu-id="e5527-244">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5527-244">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5527-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5527-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5527-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5527-246">Request</span></span>
<span data-ttu-id="e5527-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5527-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="e5527-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5527-248">Response</span></span>
<span data-ttu-id="e5527-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5527-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




