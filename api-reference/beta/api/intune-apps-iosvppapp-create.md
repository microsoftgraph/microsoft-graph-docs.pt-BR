---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86b959846225967cc4dc8315a587154f0b684d02
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790039"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="e78bd-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e78bd-103">Create iosVppApp</span></span>

<span data-ttu-id="e78bd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e78bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e78bd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e78bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e78bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e78bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e78bd-107">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="e78bd-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e78bd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e78bd-108">Prerequisites</span></span>
<span data-ttu-id="e78bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e78bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78bd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e78bd-111">Permission type</span></span>|<span data-ttu-id="e78bd-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e78bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e78bd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e78bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e78bd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78bd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e78bd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e78bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e78bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e78bd-116">Not supported.</span></span>|
|<span data-ttu-id="e78bd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e78bd-117">Application</span></span>|<span data-ttu-id="e78bd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78bd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e78bd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e78bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e78bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e78bd-120">Request headers</span></span>
|<span data-ttu-id="e78bd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e78bd-121">Header</span></span>|<span data-ttu-id="e78bd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e78bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e78bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e78bd-123">Authorization</span></span>|<span data-ttu-id="e78bd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e78bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e78bd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e78bd-125">Accept</span></span>|<span data-ttu-id="e78bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e78bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78bd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e78bd-127">Request body</span></span>
<span data-ttu-id="e78bd-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="e78bd-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="e78bd-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="e78bd-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="e78bd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e78bd-130">Property</span></span>|<span data-ttu-id="e78bd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e78bd-131">Type</span></span>|<span data-ttu-id="e78bd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e78bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e78bd-133">id</span><span class="sxs-lookup"><span data-stu-id="e78bd-133">id</span></span>|<span data-ttu-id="e78bd-134">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-134">String</span></span>|<span data-ttu-id="e78bd-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e78bd-135">Key of the entity.</span></span> <span data-ttu-id="e78bd-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e78bd-137">displayName</span></span>|<span data-ttu-id="e78bd-138">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-138">String</span></span>|<span data-ttu-id="e78bd-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e78bd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e78bd-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-141">description</span><span class="sxs-lookup"><span data-stu-id="e78bd-141">description</span></span>|<span data-ttu-id="e78bd-142">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-142">String</span></span>|<span data-ttu-id="e78bd-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-143">The description of the app.</span></span> <span data-ttu-id="e78bd-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-145">publicador</span><span class="sxs-lookup"><span data-stu-id="e78bd-145">publisher</span></span>|<span data-ttu-id="e78bd-146">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-146">String</span></span>|<span data-ttu-id="e78bd-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-147">The publisher of the app.</span></span> <span data-ttu-id="e78bd-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e78bd-149">largeIcon</span></span>|[<span data-ttu-id="e78bd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e78bd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e78bd-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e78bd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e78bd-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e78bd-153">createdDateTime</span></span>|<span data-ttu-id="e78bd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78bd-154">DateTimeOffset</span></span>|<span data-ttu-id="e78bd-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-155">The date and time the app was created.</span></span> <span data-ttu-id="e78bd-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e78bd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e78bd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78bd-158">DateTimeOffset</span></span>|<span data-ttu-id="e78bd-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e78bd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e78bd-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e78bd-161">isFeatured</span></span>|<span data-ttu-id="e78bd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e78bd-162">Boolean</span></span>|<span data-ttu-id="e78bd-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e78bd-164">privacyInformationUrl</span></span>|<span data-ttu-id="e78bd-165">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-165">String</span></span>|<span data-ttu-id="e78bd-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e78bd-166">The privacy statement Url.</span></span> <span data-ttu-id="e78bd-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e78bd-168">informationUrl</span></span>|<span data-ttu-id="e78bd-169">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-169">String</span></span>|<span data-ttu-id="e78bd-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e78bd-170">The more information Url.</span></span> <span data-ttu-id="e78bd-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-172">owner</span><span class="sxs-lookup"><span data-stu-id="e78bd-172">owner</span></span>|<span data-ttu-id="e78bd-173">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-173">String</span></span>|<span data-ttu-id="e78bd-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-174">The owner of the app.</span></span> <span data-ttu-id="e78bd-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-176">developer</span><span class="sxs-lookup"><span data-stu-id="e78bd-176">developer</span></span>|<span data-ttu-id="e78bd-177">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-177">String</span></span>|<span data-ttu-id="e78bd-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-178">The developer of the app.</span></span> <span data-ttu-id="e78bd-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-180">notes</span><span class="sxs-lookup"><span data-stu-id="e78bd-180">notes</span></span>|<span data-ttu-id="e78bd-181">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-181">String</span></span>|<span data-ttu-id="e78bd-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-182">Notes for the app.</span></span> <span data-ttu-id="e78bd-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e78bd-184">uploadState</span></span>|<span data-ttu-id="e78bd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e78bd-185">Int32</span></span>|<span data-ttu-id="e78bd-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="e78bd-186">The upload state.</span></span> <span data-ttu-id="e78bd-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="e78bd-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e78bd-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e78bd-189">publishingState</span></span>|[<span data-ttu-id="e78bd-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e78bd-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e78bd-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-191">The publishing state for the app.</span></span> <span data-ttu-id="e78bd-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e78bd-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e78bd-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e78bd-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e78bd-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e78bd-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e78bd-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e78bd-195">isAssigned</span></span>|<span data-ttu-id="e78bd-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e78bd-196">Boolean</span></span>|<span data-ttu-id="e78bd-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e78bd-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e78bd-199">roleScopeTagIds</span></span>|<span data-ttu-id="e78bd-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e78bd-200">String collection</span></span>|<span data-ttu-id="e78bd-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="e78bd-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e78bd-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e78bd-203">dependentAppCount</span></span>|<span data-ttu-id="e78bd-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e78bd-204">Int32</span></span>|<span data-ttu-id="e78bd-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="e78bd-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e78bd-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e78bd-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e78bd-207">usedLicenseCount</span></span>|<span data-ttu-id="e78bd-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e78bd-208">Int32</span></span>|<span data-ttu-id="e78bd-209">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="e78bd-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="e78bd-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e78bd-210">totalLicenseCount</span></span>|<span data-ttu-id="e78bd-211">Int32</span><span class="sxs-lookup"><span data-stu-id="e78bd-211">Int32</span></span>|<span data-ttu-id="e78bd-212">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="e78bd-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="e78bd-213">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="e78bd-213">releaseDateTime</span></span>|<span data-ttu-id="e78bd-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78bd-214">DateTimeOffset</span></span>|<span data-ttu-id="e78bd-215">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="e78bd-215">The VPP application release date and time.</span></span>|
|<span data-ttu-id="e78bd-216">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e78bd-216">appStoreUrl</span></span>|<span data-ttu-id="e78bd-217">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-217">String</span></span>|<span data-ttu-id="e78bd-218">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="e78bd-218">The store URL.</span></span>|
|<span data-ttu-id="e78bd-219">licensingType</span><span class="sxs-lookup"><span data-stu-id="e78bd-219">licensingType</span></span>|[<span data-ttu-id="e78bd-220">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e78bd-220">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="e78bd-221">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="e78bd-221">The supported License Type.</span></span>|
|<span data-ttu-id="e78bd-222">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e78bd-222">applicableDeviceType</span></span>|[<span data-ttu-id="e78bd-223">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e78bd-223">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e78bd-224">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="e78bd-224">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="e78bd-225">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e78bd-225">vppTokenOrganizationName</span></span>|<span data-ttu-id="e78bd-226">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-226">String</span></span>|<span data-ttu-id="e78bd-227">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="e78bd-227">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="e78bd-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e78bd-228">vppTokenAccountType</span></span>|[<span data-ttu-id="e78bd-229">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e78bd-229">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="e78bd-230">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="e78bd-230">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="e78bd-231">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="e78bd-231">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="e78bd-232">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="e78bd-232">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="e78bd-233">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="e78bd-233">vppTokenAppleId</span></span>|<span data-ttu-id="e78bd-234">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-234">String</span></span>|<span data-ttu-id="e78bd-235">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="e78bd-235">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="e78bd-236">bundleId</span><span class="sxs-lookup"><span data-stu-id="e78bd-236">bundleId</span></span>|<span data-ttu-id="e78bd-237">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-237">String</span></span>|<span data-ttu-id="e78bd-238">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="e78bd-238">The Identity Name.</span></span>|
|<span data-ttu-id="e78bd-239">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e78bd-239">vppTokenId</span></span>|<span data-ttu-id="e78bd-240">String</span><span class="sxs-lookup"><span data-stu-id="e78bd-240">String</span></span>|<span data-ttu-id="e78bd-241">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-241">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="e78bd-242">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="e78bd-242">revokeLicenseActionResults</span></span>|<span data-ttu-id="e78bd-243">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e78bd-243">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="e78bd-244">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e78bd-244">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="e78bd-245">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78bd-245">Response</span></span>
<span data-ttu-id="e78bd-246">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e78bd-246">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78bd-247">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e78bd-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="e78bd-248">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e78bd-248">Request</span></span>
<span data-ttu-id="e78bd-249">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e78bd-249">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e78bd-250">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78bd-250">Response</span></span>
<span data-ttu-id="e78bd-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e78bd-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



