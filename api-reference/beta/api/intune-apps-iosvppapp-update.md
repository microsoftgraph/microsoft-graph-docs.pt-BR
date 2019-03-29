---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 341e5be4f111764932ed403fd9f2b9f20e63f95b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982970"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="9d66a-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="9d66a-103">Update iosVppApp</span></span>

> <span data-ttu-id="9d66a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d66a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d66a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d66a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d66a-106">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d66a-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d66a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9d66a-107">Prerequisites</span></span>
<span data-ttu-id="9d66a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d66a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d66a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d66a-110">Permission type</span></span>|<span data-ttu-id="9d66a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9d66a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d66a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d66a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d66a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d66a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d66a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d66a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d66a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d66a-115">Not supported.</span></span>|
|<span data-ttu-id="9d66a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d66a-116">Application</span></span>|<span data-ttu-id="9d66a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d66a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d66a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d66a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9d66a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d66a-119">Request headers</span></span>
|<span data-ttu-id="9d66a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9d66a-120">Header</span></span>|<span data-ttu-id="9d66a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9d66a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d66a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d66a-122">Authorization</span></span>|<span data-ttu-id="9d66a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9d66a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d66a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9d66a-124">Accept</span></span>|<span data-ttu-id="9d66a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d66a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d66a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d66a-126">Request body</span></span>
<span data-ttu-id="9d66a-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d66a-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="9d66a-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d66a-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="9d66a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d66a-129">Property</span></span>|<span data-ttu-id="9d66a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d66a-130">Type</span></span>|<span data-ttu-id="9d66a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d66a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d66a-132">id</span><span class="sxs-lookup"><span data-stu-id="9d66a-132">id</span></span>|<span data-ttu-id="9d66a-133">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-133">String</span></span>|<span data-ttu-id="9d66a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d66a-134">Key of the entity.</span></span> <span data-ttu-id="9d66a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9d66a-136">displayName</span></span>|<span data-ttu-id="9d66a-137">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-137">String</span></span>|<span data-ttu-id="9d66a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9d66a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9d66a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-140">descrição</span><span class="sxs-lookup"><span data-stu-id="9d66a-140">description</span></span>|<span data-ttu-id="9d66a-141">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-141">String</span></span>|<span data-ttu-id="9d66a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-142">The description of the app.</span></span> <span data-ttu-id="9d66a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="9d66a-144">publisher</span></span>|<span data-ttu-id="9d66a-145">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-145">String</span></span>|<span data-ttu-id="9d66a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-146">The publisher of the app.</span></span> <span data-ttu-id="9d66a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9d66a-148">largeIcon</span></span>|[<span data-ttu-id="9d66a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9d66a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9d66a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9d66a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9d66a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d66a-152">createdDateTime</span></span>|<span data-ttu-id="9d66a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d66a-153">DateTimeOffset</span></span>|<span data-ttu-id="9d66a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-154">The date and time the app was created.</span></span> <span data-ttu-id="9d66a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d66a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9d66a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d66a-157">DateTimeOffset</span></span>|<span data-ttu-id="9d66a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9d66a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9d66a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9d66a-160">isFeatured</span></span>|<span data-ttu-id="9d66a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d66a-161">Boolean</span></span>|<span data-ttu-id="9d66a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9d66a-163">privacyInformationUrl</span></span>|<span data-ttu-id="9d66a-164">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-164">String</span></span>|<span data-ttu-id="9d66a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9d66a-165">The privacy statement Url.</span></span> <span data-ttu-id="9d66a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9d66a-167">informationUrl</span></span>|<span data-ttu-id="9d66a-168">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-168">String</span></span>|<span data-ttu-id="9d66a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9d66a-169">The more information Url.</span></span> <span data-ttu-id="9d66a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-171">owner</span><span class="sxs-lookup"><span data-stu-id="9d66a-171">owner</span></span>|<span data-ttu-id="9d66a-172">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-172">String</span></span>|<span data-ttu-id="9d66a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-173">The owner of the app.</span></span> <span data-ttu-id="9d66a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-175">developer</span><span class="sxs-lookup"><span data-stu-id="9d66a-175">developer</span></span>|<span data-ttu-id="9d66a-176">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-176">String</span></span>|<span data-ttu-id="9d66a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-177">The developer of the app.</span></span> <span data-ttu-id="9d66a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-179">notes</span><span class="sxs-lookup"><span data-stu-id="9d66a-179">notes</span></span>|<span data-ttu-id="9d66a-180">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-180">String</span></span>|<span data-ttu-id="9d66a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-181">Notes for the app.</span></span> <span data-ttu-id="9d66a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9d66a-183">uploadState</span></span>|<span data-ttu-id="9d66a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9d66a-184">Int32</span></span>|<span data-ttu-id="9d66a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="9d66a-185">The upload state.</span></span> <span data-ttu-id="9d66a-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9d66a-187">publishingState</span></span>|[<span data-ttu-id="9d66a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9d66a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9d66a-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-189">The publishing state for the app.</span></span> <span data-ttu-id="9d66a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9d66a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9d66a-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9d66a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9d66a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9d66a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9d66a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9d66a-193">isAssigned</span></span>|<span data-ttu-id="9d66a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d66a-194">Boolean</span></span>|<span data-ttu-id="9d66a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9d66a-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d66a-197">roleScopeTagIds</span></span>|<span data-ttu-id="9d66a-198">Coleção String</span><span class="sxs-lookup"><span data-stu-id="9d66a-198">String collection</span></span>|<span data-ttu-id="9d66a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9d66a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9d66a-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d66a-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9d66a-201">usedLicenseCount</span></span>|<span data-ttu-id="9d66a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9d66a-202">Int32</span></span>|<span data-ttu-id="9d66a-203">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="9d66a-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="9d66a-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9d66a-204">totalLicenseCount</span></span>|<span data-ttu-id="9d66a-205">Int32</span><span class="sxs-lookup"><span data-stu-id="9d66a-205">Int32</span></span>|<span data-ttu-id="9d66a-206">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="9d66a-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="9d66a-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="9d66a-207">releaseDateTime</span></span>|<span data-ttu-id="9d66a-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d66a-208">DateTimeOffset</span></span>|<span data-ttu-id="9d66a-209">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="9d66a-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="9d66a-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9d66a-210">appStoreUrl</span></span>|<span data-ttu-id="9d66a-211">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-211">String</span></span>|<span data-ttu-id="9d66a-212">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="9d66a-212">The store URL.</span></span>|
|<span data-ttu-id="9d66a-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="9d66a-213">licensingType</span></span>|[<span data-ttu-id="9d66a-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="9d66a-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="9d66a-215">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="9d66a-215">The supported License Type.</span></span>|
|<span data-ttu-id="9d66a-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9d66a-216">applicableDeviceType</span></span>|[<span data-ttu-id="9d66a-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9d66a-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9d66a-218">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="9d66a-218">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="9d66a-219">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="9d66a-219">vppTokenOrganizationName</span></span>|<span data-ttu-id="9d66a-220">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-220">String</span></span>|<span data-ttu-id="9d66a-221">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="9d66a-221">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="9d66a-222">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9d66a-222">vppTokenAccountType</span></span>|[<span data-ttu-id="9d66a-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9d66a-223">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="9d66a-224">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="9d66a-224">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="9d66a-225">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="9d66a-225">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="9d66a-226">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="9d66a-226">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="9d66a-227">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="9d66a-227">vppTokenAppleId</span></span>|<span data-ttu-id="9d66a-228">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-228">String</span></span>|<span data-ttu-id="9d66a-229">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="9d66a-229">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9d66a-230">bundleId</span><span class="sxs-lookup"><span data-stu-id="9d66a-230">bundleId</span></span>|<span data-ttu-id="9d66a-231">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-231">String</span></span>|<span data-ttu-id="9d66a-232">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9d66a-232">The Identity Name.</span></span>|
|<span data-ttu-id="9d66a-233">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="9d66a-233">vppTokenId</span></span>|<span data-ttu-id="9d66a-234">String</span><span class="sxs-lookup"><span data-stu-id="9d66a-234">String</span></span>|<span data-ttu-id="9d66a-235">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-235">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="9d66a-236">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="9d66a-236">revokeLicenseActionResults</span></span>|<span data-ttu-id="9d66a-237">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9d66a-237">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="9d66a-238">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9d66a-238">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="9d66a-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d66a-239">Response</span></span>
<span data-ttu-id="9d66a-240">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d66a-240">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d66a-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d66a-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d66a-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d66a-242">Request</span></span>
<span data-ttu-id="9d66a-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9d66a-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1972

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

### <a name="response"></a><span data-ttu-id="9d66a-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d66a-244">Response</span></span>
<span data-ttu-id="9d66a-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d66a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2144

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




