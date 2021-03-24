---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c071739260d207ad6e7d4b92392fa105190b7cdd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140690"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="310c7-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="310c7-103">Create iosVppApp</span></span>

<span data-ttu-id="310c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="310c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="310c7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="310c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="310c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="310c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="310c7-107">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="310c7-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="310c7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="310c7-108">Prerequisites</span></span>
<span data-ttu-id="310c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="310c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="310c7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="310c7-111">Permission type</span></span>|<span data-ttu-id="310c7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="310c7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="310c7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="310c7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="310c7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310c7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="310c7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="310c7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="310c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="310c7-116">Not supported.</span></span>|
|<span data-ttu-id="310c7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="310c7-117">Application</span></span>|<span data-ttu-id="310c7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="310c7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="310c7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="310c7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="310c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="310c7-120">Request headers</span></span>
|<span data-ttu-id="310c7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="310c7-121">Header</span></span>|<span data-ttu-id="310c7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="310c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="310c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="310c7-123">Authorization</span></span>|<span data-ttu-id="310c7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="310c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="310c7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="310c7-125">Accept</span></span>|<span data-ttu-id="310c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="310c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="310c7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="310c7-127">Request body</span></span>
<span data-ttu-id="310c7-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="310c7-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="310c7-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="310c7-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="310c7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="310c7-130">Property</span></span>|<span data-ttu-id="310c7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="310c7-131">Type</span></span>|<span data-ttu-id="310c7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="310c7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="310c7-133">id</span><span class="sxs-lookup"><span data-stu-id="310c7-133">id</span></span>|<span data-ttu-id="310c7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-134">String</span></span>|<span data-ttu-id="310c7-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="310c7-135">Key of the entity.</span></span> <span data-ttu-id="310c7-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="310c7-137">displayName</span></span>|<span data-ttu-id="310c7-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-138">String</span></span>|<span data-ttu-id="310c7-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="310c7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="310c7-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-141">descrição</span><span class="sxs-lookup"><span data-stu-id="310c7-141">description</span></span>|<span data-ttu-id="310c7-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-142">String</span></span>|<span data-ttu-id="310c7-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-143">The description of the app.</span></span> <span data-ttu-id="310c7-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-145">publicador</span><span class="sxs-lookup"><span data-stu-id="310c7-145">publisher</span></span>|<span data-ttu-id="310c7-146">String</span><span class="sxs-lookup"><span data-stu-id="310c7-146">String</span></span>|<span data-ttu-id="310c7-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-147">The publisher of the app.</span></span> <span data-ttu-id="310c7-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="310c7-149">largeIcon</span></span>|[<span data-ttu-id="310c7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="310c7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="310c7-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="310c7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="310c7-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="310c7-153">createdDateTime</span></span>|<span data-ttu-id="310c7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="310c7-154">DateTimeOffset</span></span>|<span data-ttu-id="310c7-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-155">The date and time the app was created.</span></span> <span data-ttu-id="310c7-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="310c7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="310c7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="310c7-158">DateTimeOffset</span></span>|<span data-ttu-id="310c7-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="310c7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="310c7-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="310c7-161">isFeatured</span></span>|<span data-ttu-id="310c7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="310c7-162">Boolean</span></span>|<span data-ttu-id="310c7-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="310c7-164">privacyInformationUrl</span></span>|<span data-ttu-id="310c7-165">String</span><span class="sxs-lookup"><span data-stu-id="310c7-165">String</span></span>|<span data-ttu-id="310c7-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="310c7-166">The privacy statement Url.</span></span> <span data-ttu-id="310c7-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="310c7-168">informationUrl</span></span>|<span data-ttu-id="310c7-169">String</span><span class="sxs-lookup"><span data-stu-id="310c7-169">String</span></span>|<span data-ttu-id="310c7-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="310c7-170">The more information Url.</span></span> <span data-ttu-id="310c7-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-172">owner</span><span class="sxs-lookup"><span data-stu-id="310c7-172">owner</span></span>|<span data-ttu-id="310c7-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-173">String</span></span>|<span data-ttu-id="310c7-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="310c7-174">The owner of the app.</span></span> <span data-ttu-id="310c7-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-176">developer</span><span class="sxs-lookup"><span data-stu-id="310c7-176">developer</span></span>|<span data-ttu-id="310c7-177">String</span><span class="sxs-lookup"><span data-stu-id="310c7-177">String</span></span>|<span data-ttu-id="310c7-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-178">The developer of the app.</span></span> <span data-ttu-id="310c7-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-180">notes</span><span class="sxs-lookup"><span data-stu-id="310c7-180">notes</span></span>|<span data-ttu-id="310c7-181">String</span><span class="sxs-lookup"><span data-stu-id="310c7-181">String</span></span>|<span data-ttu-id="310c7-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-182">Notes for the app.</span></span> <span data-ttu-id="310c7-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="310c7-184">uploadState</span></span>|<span data-ttu-id="310c7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-185">Int32</span></span>|<span data-ttu-id="310c7-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="310c7-186">The upload state.</span></span> <span data-ttu-id="310c7-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="310c7-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="310c7-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="310c7-189">publishingState</span></span>|[<span data-ttu-id="310c7-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="310c7-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="310c7-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-191">The publishing state for the app.</span></span> <span data-ttu-id="310c7-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="310c7-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="310c7-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="310c7-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="310c7-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="310c7-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="310c7-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="310c7-195">isAssigned</span></span>|<span data-ttu-id="310c7-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="310c7-196">Boolean</span></span>|<span data-ttu-id="310c7-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="310c7-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="310c7-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="310c7-199">roleScopeTagIds</span></span>|<span data-ttu-id="310c7-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-200">String collection</span></span>|<span data-ttu-id="310c7-201">Lista de ids de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="310c7-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="310c7-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="310c7-203">dependentAppCount</span></span>|<span data-ttu-id="310c7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-204">Int32</span></span>|<span data-ttu-id="310c7-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="310c7-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="310c7-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="310c7-207">supersedingAppCount</span></span>|<span data-ttu-id="310c7-208">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-208">Int32</span></span>|<span data-ttu-id="310c7-209">O número total de aplicativos que esse aplicativo sobressede direta ou indiretamente.</span><span class="sxs-lookup"><span data-stu-id="310c7-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="310c7-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="310c7-211">supersededAppCount</span></span>|<span data-ttu-id="310c7-212">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-212">Int32</span></span>|<span data-ttu-id="310c7-213">O número total de aplicativos pelos quais esse aplicativo é, direta ou indiretamente, é suplido.</span><span class="sxs-lookup"><span data-stu-id="310c7-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="310c7-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="310c7-215">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="310c7-215">usedLicenseCount</span></span>|<span data-ttu-id="310c7-216">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-216">Int32</span></span>|<span data-ttu-id="310c7-217">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="310c7-217">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="310c7-218">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="310c7-218">totalLicenseCount</span></span>|<span data-ttu-id="310c7-219">Int32</span><span class="sxs-lookup"><span data-stu-id="310c7-219">Int32</span></span>|<span data-ttu-id="310c7-220">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="310c7-220">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="310c7-221">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="310c7-221">releaseDateTime</span></span>|<span data-ttu-id="310c7-222">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="310c7-222">DateTimeOffset</span></span>|<span data-ttu-id="310c7-223">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="310c7-223">The VPP application release date and time.</span></span>|
|<span data-ttu-id="310c7-224">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="310c7-224">appStoreUrl</span></span>|<span data-ttu-id="310c7-225">String</span><span class="sxs-lookup"><span data-stu-id="310c7-225">String</span></span>|<span data-ttu-id="310c7-226">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="310c7-226">The store URL.</span></span>|
|<span data-ttu-id="310c7-227">licensingType</span><span class="sxs-lookup"><span data-stu-id="310c7-227">licensingType</span></span>|[<span data-ttu-id="310c7-228">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="310c7-228">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="310c7-229">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="310c7-229">The supported License Type.</span></span>|
|<span data-ttu-id="310c7-230">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="310c7-230">applicableDeviceType</span></span>|[<span data-ttu-id="310c7-231">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="310c7-231">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="310c7-232">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="310c7-232">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="310c7-233">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="310c7-233">vppTokenOrganizationName</span></span>|<span data-ttu-id="310c7-234">String</span><span class="sxs-lookup"><span data-stu-id="310c7-234">String</span></span>|<span data-ttu-id="310c7-235">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="310c7-235">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="310c7-236">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="310c7-236">vppTokenAccountType</span></span>|[<span data-ttu-id="310c7-237">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="310c7-237">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="310c7-238">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="310c7-238">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="310c7-239">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="310c7-239">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="310c7-240">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="310c7-240">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="310c7-241">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="310c7-241">vppTokenAppleId</span></span>|<span data-ttu-id="310c7-242">String</span><span class="sxs-lookup"><span data-stu-id="310c7-242">String</span></span>|<span data-ttu-id="310c7-243">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="310c7-243">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="310c7-244">bundleId</span><span class="sxs-lookup"><span data-stu-id="310c7-244">bundleId</span></span>|<span data-ttu-id="310c7-245">String</span><span class="sxs-lookup"><span data-stu-id="310c7-245">String</span></span>|<span data-ttu-id="310c7-246">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="310c7-246">The Identity Name.</span></span>|
|<span data-ttu-id="310c7-247">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="310c7-247">vppTokenId</span></span>|<span data-ttu-id="310c7-248">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="310c7-248">String</span></span>|<span data-ttu-id="310c7-249">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-249">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="310c7-250">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="310c7-250">revokeLicenseActionResults</span></span>|<span data-ttu-id="310c7-251">[Coleção iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="310c7-251">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="310c7-252">Resultados de revogar ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="310c7-252">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="310c7-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="310c7-253">Response</span></span>
<span data-ttu-id="310c7-254">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="310c7-254">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="310c7-255">Exemplo</span><span class="sxs-lookup"><span data-stu-id="310c7-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="310c7-256">Solicitação</span><span class="sxs-lookup"><span data-stu-id="310c7-256">Request</span></span>
<span data-ttu-id="310c7-257">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="310c7-257">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2056

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="310c7-258">Resposta</span><span class="sxs-lookup"><span data-stu-id="310c7-258">Response</span></span>
<span data-ttu-id="310c7-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="310c7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2228

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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




