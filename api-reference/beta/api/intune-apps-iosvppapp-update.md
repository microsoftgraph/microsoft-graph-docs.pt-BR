---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7d3f27c4304fa7b2becd5ed3db4801b80a3c963
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416727"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="1b201-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="1b201-103">Update iosVppApp</span></span>

<span data-ttu-id="1b201-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b201-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b201-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b201-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b201-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b201-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b201-107">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b201-107">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b201-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1b201-108">Prerequisites</span></span>
<span data-ttu-id="1b201-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b201-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b201-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b201-111">Permission type</span></span>|<span data-ttu-id="1b201-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1b201-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b201-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b201-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b201-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b201-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b201-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b201-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b201-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b201-116">Not supported.</span></span>|
|<span data-ttu-id="1b201-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b201-117">Application</span></span>|<span data-ttu-id="1b201-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b201-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b201-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b201-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1b201-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b201-120">Request headers</span></span>
|<span data-ttu-id="1b201-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1b201-121">Header</span></span>|<span data-ttu-id="1b201-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1b201-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b201-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b201-123">Authorization</span></span>|<span data-ttu-id="1b201-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b201-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b201-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1b201-125">Accept</span></span>|<span data-ttu-id="1b201-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b201-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b201-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b201-127">Request body</span></span>
<span data-ttu-id="1b201-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b201-128">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="1b201-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b201-129">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="1b201-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b201-130">Property</span></span>|<span data-ttu-id="1b201-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b201-131">Type</span></span>|<span data-ttu-id="1b201-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b201-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b201-133">id</span><span class="sxs-lookup"><span data-stu-id="1b201-133">id</span></span>|<span data-ttu-id="1b201-134">String</span><span class="sxs-lookup"><span data-stu-id="1b201-134">String</span></span>|<span data-ttu-id="1b201-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1b201-135">Key of the entity.</span></span> <span data-ttu-id="1b201-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1b201-137">displayName</span></span>|<span data-ttu-id="1b201-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b201-138">String</span></span>|<span data-ttu-id="1b201-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="1b201-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1b201-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-141">description</span><span class="sxs-lookup"><span data-stu-id="1b201-141">description</span></span>|<span data-ttu-id="1b201-142">String</span><span class="sxs-lookup"><span data-stu-id="1b201-142">String</span></span>|<span data-ttu-id="1b201-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-143">The description of the app.</span></span> <span data-ttu-id="1b201-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-145">publicador</span><span class="sxs-lookup"><span data-stu-id="1b201-145">publisher</span></span>|<span data-ttu-id="1b201-146">String</span><span class="sxs-lookup"><span data-stu-id="1b201-146">String</span></span>|<span data-ttu-id="1b201-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-147">The publisher of the app.</span></span> <span data-ttu-id="1b201-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1b201-149">largeIcon</span></span>|[<span data-ttu-id="1b201-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b201-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1b201-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="1b201-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1b201-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b201-153">createdDateTime</span></span>|<span data-ttu-id="1b201-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b201-154">DateTimeOffset</span></span>|<span data-ttu-id="1b201-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-155">The date and time the app was created.</span></span> <span data-ttu-id="1b201-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b201-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1b201-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b201-158">DateTimeOffset</span></span>|<span data-ttu-id="1b201-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1b201-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1b201-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1b201-161">isFeatured</span></span>|<span data-ttu-id="1b201-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b201-162">Boolean</span></span>|<span data-ttu-id="1b201-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1b201-164">privacyInformationUrl</span></span>|<span data-ttu-id="1b201-165">String</span><span class="sxs-lookup"><span data-stu-id="1b201-165">String</span></span>|<span data-ttu-id="1b201-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="1b201-166">The privacy statement Url.</span></span> <span data-ttu-id="1b201-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1b201-168">informationUrl</span></span>|<span data-ttu-id="1b201-169">String</span><span class="sxs-lookup"><span data-stu-id="1b201-169">String</span></span>|<span data-ttu-id="1b201-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="1b201-170">The more information Url.</span></span> <span data-ttu-id="1b201-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-172">owner</span><span class="sxs-lookup"><span data-stu-id="1b201-172">owner</span></span>|<span data-ttu-id="1b201-173">String</span><span class="sxs-lookup"><span data-stu-id="1b201-173">String</span></span>|<span data-ttu-id="1b201-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="1b201-174">The owner of the app.</span></span> <span data-ttu-id="1b201-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-176">developer</span><span class="sxs-lookup"><span data-stu-id="1b201-176">developer</span></span>|<span data-ttu-id="1b201-177">String</span><span class="sxs-lookup"><span data-stu-id="1b201-177">String</span></span>|<span data-ttu-id="1b201-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-178">The developer of the app.</span></span> <span data-ttu-id="1b201-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-180">notes</span><span class="sxs-lookup"><span data-stu-id="1b201-180">notes</span></span>|<span data-ttu-id="1b201-181">String</span><span class="sxs-lookup"><span data-stu-id="1b201-181">String</span></span>|<span data-ttu-id="1b201-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-182">Notes for the app.</span></span> <span data-ttu-id="1b201-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1b201-184">uploadState</span></span>|<span data-ttu-id="1b201-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1b201-185">Int32</span></span>|<span data-ttu-id="1b201-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="1b201-186">The upload state.</span></span> <span data-ttu-id="1b201-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b201-188">publishingState</span></span>|[<span data-ttu-id="1b201-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1b201-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1b201-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-190">The publishing state for the app.</span></span> <span data-ttu-id="1b201-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="1b201-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1b201-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="1b201-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="1b201-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="1b201-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1b201-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1b201-194">isAssigned</span></span>|<span data-ttu-id="1b201-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b201-195">Boolean</span></span>|<span data-ttu-id="1b201-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="1b201-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1b201-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1b201-198">roleScopeTagIds</span></span>|<span data-ttu-id="1b201-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1b201-199">String collection</span></span>|<span data-ttu-id="1b201-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="1b201-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1b201-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="1b201-202">dependentAppCount</span></span>|<span data-ttu-id="1b201-203">Int32</span><span class="sxs-lookup"><span data-stu-id="1b201-203">Int32</span></span>|<span data-ttu-id="1b201-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="1b201-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="1b201-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="1b201-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1b201-206">usedLicenseCount</span></span>|<span data-ttu-id="1b201-207">Int32</span><span class="sxs-lookup"><span data-stu-id="1b201-207">Int32</span></span>|<span data-ttu-id="1b201-208">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="1b201-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1b201-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1b201-209">totalLicenseCount</span></span>|<span data-ttu-id="1b201-210">Int32</span><span class="sxs-lookup"><span data-stu-id="1b201-210">Int32</span></span>|<span data-ttu-id="1b201-211">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="1b201-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1b201-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1b201-212">releaseDateTime</span></span>|<span data-ttu-id="1b201-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b201-213">DateTimeOffset</span></span>|<span data-ttu-id="1b201-214">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="1b201-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="1b201-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1b201-215">appStoreUrl</span></span>|<span data-ttu-id="1b201-216">String</span><span class="sxs-lookup"><span data-stu-id="1b201-216">String</span></span>|<span data-ttu-id="1b201-217">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="1b201-217">The store URL.</span></span>|
|<span data-ttu-id="1b201-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="1b201-218">licensingType</span></span>|[<span data-ttu-id="1b201-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1b201-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1b201-220">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="1b201-220">The supported License Type.</span></span>|
|<span data-ttu-id="1b201-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1b201-221">applicableDeviceType</span></span>|[<span data-ttu-id="1b201-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1b201-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1b201-223">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="1b201-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="1b201-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1b201-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="1b201-225">String</span><span class="sxs-lookup"><span data-stu-id="1b201-225">String</span></span>|<span data-ttu-id="1b201-226">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="1b201-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="1b201-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1b201-227">vppTokenAccountType</span></span>|[<span data-ttu-id="1b201-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1b201-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="1b201-229">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="1b201-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="1b201-230">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="1b201-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="1b201-231">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="1b201-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="1b201-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="1b201-232">vppTokenAppleId</span></span>|<span data-ttu-id="1b201-233">String</span><span class="sxs-lookup"><span data-stu-id="1b201-233">String</span></span>|<span data-ttu-id="1b201-234">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="1b201-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1b201-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="1b201-235">bundleId</span></span>|<span data-ttu-id="1b201-236">String</span><span class="sxs-lookup"><span data-stu-id="1b201-236">String</span></span>|<span data-ttu-id="1b201-237">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1b201-237">The Identity Name.</span></span>|
|<span data-ttu-id="1b201-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="1b201-238">vppTokenId</span></span>|<span data-ttu-id="1b201-239">String</span><span class="sxs-lookup"><span data-stu-id="1b201-239">String</span></span>|<span data-ttu-id="1b201-240">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="1b201-241">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="1b201-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="1b201-242">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="1b201-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="1b201-243">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b201-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="1b201-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b201-244">Response</span></span>
<span data-ttu-id="1b201-245">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b201-245">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b201-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1b201-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b201-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b201-247">Request</span></span>
<span data-ttu-id="1b201-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b201-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1b201-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b201-249">Response</span></span>
<span data-ttu-id="1b201-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b201-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



