---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3136e5ba079dbea1e876cf13245d8733b3952377
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394583"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="39050-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="39050-103">Create iosVppApp</span></span>

<span data-ttu-id="39050-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39050-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39050-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39050-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39050-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39050-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39050-107">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="39050-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39050-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="39050-108">Prerequisites</span></span>
<span data-ttu-id="39050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39050-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39050-111">Permission type</span></span>|<span data-ttu-id="39050-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="39050-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39050-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39050-113">Delegated (work or school account)</span></span>|<span data-ttu-id="39050-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39050-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39050-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39050-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39050-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39050-116">Not supported.</span></span>|
|<span data-ttu-id="39050-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39050-117">Application</span></span>|<span data-ttu-id="39050-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39050-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39050-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39050-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="39050-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39050-120">Request headers</span></span>
|<span data-ttu-id="39050-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39050-121">Header</span></span>|<span data-ttu-id="39050-122">Valor</span><span class="sxs-lookup"><span data-stu-id="39050-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39050-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="39050-123">Authorization</span></span>|<span data-ttu-id="39050-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39050-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39050-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="39050-125">Accept</span></span>|<span data-ttu-id="39050-126">application/json</span><span class="sxs-lookup"><span data-stu-id="39050-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39050-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39050-127">Request body</span></span>
<span data-ttu-id="39050-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="39050-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="39050-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="39050-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="39050-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39050-130">Property</span></span>|<span data-ttu-id="39050-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="39050-131">Type</span></span>|<span data-ttu-id="39050-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="39050-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39050-133">id</span><span class="sxs-lookup"><span data-stu-id="39050-133">id</span></span>|<span data-ttu-id="39050-134">String</span><span class="sxs-lookup"><span data-stu-id="39050-134">String</span></span>|<span data-ttu-id="39050-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="39050-135">Key of the entity.</span></span> <span data-ttu-id="39050-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-137">displayName</span><span class="sxs-lookup"><span data-stu-id="39050-137">displayName</span></span>|<span data-ttu-id="39050-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39050-138">String</span></span>|<span data-ttu-id="39050-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="39050-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="39050-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-141">description</span><span class="sxs-lookup"><span data-stu-id="39050-141">description</span></span>|<span data-ttu-id="39050-142">String</span><span class="sxs-lookup"><span data-stu-id="39050-142">String</span></span>|<span data-ttu-id="39050-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-143">The description of the app.</span></span> <span data-ttu-id="39050-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-145">publicador</span><span class="sxs-lookup"><span data-stu-id="39050-145">publisher</span></span>|<span data-ttu-id="39050-146">String</span><span class="sxs-lookup"><span data-stu-id="39050-146">String</span></span>|<span data-ttu-id="39050-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-147">The publisher of the app.</span></span> <span data-ttu-id="39050-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="39050-149">largeIcon</span></span>|[<span data-ttu-id="39050-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="39050-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="39050-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="39050-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="39050-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="39050-153">createdDateTime</span></span>|<span data-ttu-id="39050-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39050-154">DateTimeOffset</span></span>|<span data-ttu-id="39050-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-155">The date and time the app was created.</span></span> <span data-ttu-id="39050-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="39050-157">lastModifiedDateTime</span></span>|<span data-ttu-id="39050-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39050-158">DateTimeOffset</span></span>|<span data-ttu-id="39050-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="39050-159">The date and time the app was last modified.</span></span> <span data-ttu-id="39050-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="39050-161">isFeatured</span></span>|<span data-ttu-id="39050-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="39050-162">Boolean</span></span>|<span data-ttu-id="39050-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="39050-164">privacyInformationUrl</span></span>|<span data-ttu-id="39050-165">String</span><span class="sxs-lookup"><span data-stu-id="39050-165">String</span></span>|<span data-ttu-id="39050-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="39050-166">The privacy statement Url.</span></span> <span data-ttu-id="39050-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="39050-168">informationUrl</span></span>|<span data-ttu-id="39050-169">String</span><span class="sxs-lookup"><span data-stu-id="39050-169">String</span></span>|<span data-ttu-id="39050-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="39050-170">The more information Url.</span></span> <span data-ttu-id="39050-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-172">owner</span><span class="sxs-lookup"><span data-stu-id="39050-172">owner</span></span>|<span data-ttu-id="39050-173">String</span><span class="sxs-lookup"><span data-stu-id="39050-173">String</span></span>|<span data-ttu-id="39050-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="39050-174">The owner of the app.</span></span> <span data-ttu-id="39050-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-176">developer</span><span class="sxs-lookup"><span data-stu-id="39050-176">developer</span></span>|<span data-ttu-id="39050-177">String</span><span class="sxs-lookup"><span data-stu-id="39050-177">String</span></span>|<span data-ttu-id="39050-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-178">The developer of the app.</span></span> <span data-ttu-id="39050-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-180">notes</span><span class="sxs-lookup"><span data-stu-id="39050-180">notes</span></span>|<span data-ttu-id="39050-181">String</span><span class="sxs-lookup"><span data-stu-id="39050-181">String</span></span>|<span data-ttu-id="39050-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-182">Notes for the app.</span></span> <span data-ttu-id="39050-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="39050-184">uploadState</span></span>|<span data-ttu-id="39050-185">Int32</span><span class="sxs-lookup"><span data-stu-id="39050-185">Int32</span></span>|<span data-ttu-id="39050-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="39050-186">The upload state.</span></span> <span data-ttu-id="39050-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="39050-188">publishingState</span></span>|[<span data-ttu-id="39050-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="39050-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="39050-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-190">The publishing state for the app.</span></span> <span data-ttu-id="39050-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="39050-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="39050-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="39050-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="39050-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="39050-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="39050-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="39050-194">isAssigned</span></span>|<span data-ttu-id="39050-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="39050-195">Boolean</span></span>|<span data-ttu-id="39050-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="39050-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="39050-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="39050-198">roleScopeTagIds</span></span>|<span data-ttu-id="39050-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="39050-199">String collection</span></span>|<span data-ttu-id="39050-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="39050-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="39050-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="39050-202">dependentAppCount</span></span>|<span data-ttu-id="39050-203">Int32</span><span class="sxs-lookup"><span data-stu-id="39050-203">Int32</span></span>|<span data-ttu-id="39050-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="39050-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="39050-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="39050-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="39050-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="39050-206">usedLicenseCount</span></span>|<span data-ttu-id="39050-207">Int32</span><span class="sxs-lookup"><span data-stu-id="39050-207">Int32</span></span>|<span data-ttu-id="39050-208">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="39050-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="39050-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="39050-209">totalLicenseCount</span></span>|<span data-ttu-id="39050-210">Int32</span><span class="sxs-lookup"><span data-stu-id="39050-210">Int32</span></span>|<span data-ttu-id="39050-211">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="39050-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="39050-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="39050-212">releaseDateTime</span></span>|<span data-ttu-id="39050-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39050-213">DateTimeOffset</span></span>|<span data-ttu-id="39050-214">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="39050-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="39050-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="39050-215">appStoreUrl</span></span>|<span data-ttu-id="39050-216">String</span><span class="sxs-lookup"><span data-stu-id="39050-216">String</span></span>|<span data-ttu-id="39050-217">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="39050-217">The store URL.</span></span>|
|<span data-ttu-id="39050-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="39050-218">licensingType</span></span>|[<span data-ttu-id="39050-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="39050-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="39050-220">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="39050-220">The supported License Type.</span></span>|
|<span data-ttu-id="39050-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="39050-221">applicableDeviceType</span></span>|[<span data-ttu-id="39050-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="39050-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="39050-223">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="39050-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="39050-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="39050-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="39050-225">String</span><span class="sxs-lookup"><span data-stu-id="39050-225">String</span></span>|<span data-ttu-id="39050-226">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="39050-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="39050-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="39050-227">vppTokenAccountType</span></span>|[<span data-ttu-id="39050-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="39050-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="39050-229">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="39050-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="39050-230">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="39050-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="39050-231">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="39050-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="39050-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="39050-232">vppTokenAppleId</span></span>|<span data-ttu-id="39050-233">String</span><span class="sxs-lookup"><span data-stu-id="39050-233">String</span></span>|<span data-ttu-id="39050-234">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="39050-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="39050-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="39050-235">bundleId</span></span>|<span data-ttu-id="39050-236">String</span><span class="sxs-lookup"><span data-stu-id="39050-236">String</span></span>|<span data-ttu-id="39050-237">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="39050-237">The Identity Name.</span></span>|
|<span data-ttu-id="39050-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="39050-238">vppTokenId</span></span>|<span data-ttu-id="39050-239">String</span><span class="sxs-lookup"><span data-stu-id="39050-239">String</span></span>|<span data-ttu-id="39050-240">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="39050-241">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="39050-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="39050-242">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="39050-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="39050-243">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39050-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="39050-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="39050-244">Response</span></span>
<span data-ttu-id="39050-245">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39050-245">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39050-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39050-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="39050-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39050-247">Request</span></span>
<span data-ttu-id="39050-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="39050-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39050-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="39050-249">Response</span></span>
<span data-ttu-id="39050-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39050-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



