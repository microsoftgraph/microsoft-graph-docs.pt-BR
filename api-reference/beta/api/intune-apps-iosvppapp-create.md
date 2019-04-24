---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ff4d6bc75e82d4d734bd07e0785965e75bfe61d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495677"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="6cdcc-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="6cdcc-103">Create iosVppApp</span></span>

> <span data-ttu-id="6cdcc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cdcc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cdcc-106">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cdcc-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cdcc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6cdcc-107">Prerequisites</span></span>
<span data-ttu-id="6cdcc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cdcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cdcc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6cdcc-110">Permission type</span></span>|<span data-ttu-id="6cdcc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cdcc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6cdcc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cdcc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cdcc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cdcc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-115">Not supported.</span></span>|
|<span data-ttu-id="6cdcc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6cdcc-116">Application</span></span>|<span data-ttu-id="6cdcc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cdcc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6cdcc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6cdcc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdcc-119">Request headers</span></span>
|<span data-ttu-id="6cdcc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6cdcc-120">Header</span></span>|<span data-ttu-id="6cdcc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6cdcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cdcc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6cdcc-122">Authorization</span></span>|<span data-ttu-id="6cdcc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cdcc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6cdcc-124">Accept</span></span>|<span data-ttu-id="6cdcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cdcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cdcc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdcc-126">Request body</span></span>
<span data-ttu-id="6cdcc-127">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="6cdcc-128">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="6cdcc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cdcc-129">Property</span></span>|<span data-ttu-id="6cdcc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cdcc-130">Type</span></span>|<span data-ttu-id="6cdcc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cdcc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cdcc-132">id</span><span class="sxs-lookup"><span data-stu-id="6cdcc-132">id</span></span>|<span data-ttu-id="6cdcc-133">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-133">String</span></span>|<span data-ttu-id="6cdcc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-134">Key of the entity.</span></span> <span data-ttu-id="6cdcc-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6cdcc-136">displayName</span></span>|<span data-ttu-id="6cdcc-137">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-137">String</span></span>|<span data-ttu-id="6cdcc-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6cdcc-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-140">description</span><span class="sxs-lookup"><span data-stu-id="6cdcc-140">description</span></span>|<span data-ttu-id="6cdcc-141">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-141">String</span></span>|<span data-ttu-id="6cdcc-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-142">The description of the app.</span></span> <span data-ttu-id="6cdcc-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-144">publicador</span><span class="sxs-lookup"><span data-stu-id="6cdcc-144">publisher</span></span>|<span data-ttu-id="6cdcc-145">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-145">String</span></span>|<span data-ttu-id="6cdcc-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-146">The publisher of the app.</span></span> <span data-ttu-id="6cdcc-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6cdcc-148">largeIcon</span></span>|[<span data-ttu-id="6cdcc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6cdcc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6cdcc-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6cdcc-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdcc-152">createdDateTime</span></span>|<span data-ttu-id="6cdcc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cdcc-153">DateTimeOffset</span></span>|<span data-ttu-id="6cdcc-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-154">The date and time the app was created.</span></span> <span data-ttu-id="6cdcc-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdcc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6cdcc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cdcc-157">DateTimeOffset</span></span>|<span data-ttu-id="6cdcc-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6cdcc-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6cdcc-160">isFeatured</span></span>|<span data-ttu-id="6cdcc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cdcc-161">Boolean</span></span>|<span data-ttu-id="6cdcc-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6cdcc-163">privacyInformationUrl</span></span>|<span data-ttu-id="6cdcc-164">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-164">String</span></span>|<span data-ttu-id="6cdcc-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-165">The privacy statement Url.</span></span> <span data-ttu-id="6cdcc-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6cdcc-167">informationUrl</span></span>|<span data-ttu-id="6cdcc-168">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-168">String</span></span>|<span data-ttu-id="6cdcc-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-169">The more information Url.</span></span> <span data-ttu-id="6cdcc-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-171">owner</span><span class="sxs-lookup"><span data-stu-id="6cdcc-171">owner</span></span>|<span data-ttu-id="6cdcc-172">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-172">String</span></span>|<span data-ttu-id="6cdcc-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-173">The owner of the app.</span></span> <span data-ttu-id="6cdcc-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-175">developer</span><span class="sxs-lookup"><span data-stu-id="6cdcc-175">developer</span></span>|<span data-ttu-id="6cdcc-176">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-176">String</span></span>|<span data-ttu-id="6cdcc-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-177">The developer of the app.</span></span> <span data-ttu-id="6cdcc-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-179">notes</span><span class="sxs-lookup"><span data-stu-id="6cdcc-179">notes</span></span>|<span data-ttu-id="6cdcc-180">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-180">String</span></span>|<span data-ttu-id="6cdcc-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-181">Notes for the app.</span></span> <span data-ttu-id="6cdcc-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6cdcc-183">uploadState</span></span>|<span data-ttu-id="6cdcc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6cdcc-184">Int32</span></span>|<span data-ttu-id="6cdcc-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-185">The upload state.</span></span> <span data-ttu-id="6cdcc-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6cdcc-187">publishingState</span></span>|[<span data-ttu-id="6cdcc-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6cdcc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6cdcc-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-189">The publishing state for the app.</span></span> <span data-ttu-id="6cdcc-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6cdcc-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="6cdcc-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6cdcc-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6cdcc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6cdcc-193">isAssigned</span></span>|<span data-ttu-id="6cdcc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cdcc-194">Boolean</span></span>|<span data-ttu-id="6cdcc-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6cdcc-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6cdcc-197">roleScopeTagIds</span></span>|<span data-ttu-id="6cdcc-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cdcc-198">String collection</span></span>|<span data-ttu-id="6cdcc-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6cdcc-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6cdcc-201">dependentAppCount</span></span>|<span data-ttu-id="6cdcc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6cdcc-202">Int32</span></span>|<span data-ttu-id="6cdcc-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6cdcc-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6cdcc-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6cdcc-205">usedLicenseCount</span></span>|<span data-ttu-id="6cdcc-206">Int32</span><span class="sxs-lookup"><span data-stu-id="6cdcc-206">Int32</span></span>|<span data-ttu-id="6cdcc-207">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="6cdcc-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="6cdcc-208">totalLicenseCount</span></span>|<span data-ttu-id="6cdcc-209">Int32</span><span class="sxs-lookup"><span data-stu-id="6cdcc-209">Int32</span></span>|<span data-ttu-id="6cdcc-210">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="6cdcc-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="6cdcc-211">releaseDateTime</span></span>|<span data-ttu-id="6cdcc-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cdcc-212">DateTimeOffset</span></span>|<span data-ttu-id="6cdcc-213">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="6cdcc-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6cdcc-214">appStoreUrl</span></span>|<span data-ttu-id="6cdcc-215">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-215">String</span></span>|<span data-ttu-id="6cdcc-216">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-216">The store URL.</span></span>|
|<span data-ttu-id="6cdcc-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-217">licensingType</span></span>|[<span data-ttu-id="6cdcc-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="6cdcc-219">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-219">The supported License Type.</span></span>|
|<span data-ttu-id="6cdcc-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-220">applicableDeviceType</span></span>|[<span data-ttu-id="6cdcc-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="6cdcc-222">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="6cdcc-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="6cdcc-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="6cdcc-224">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-224">String</span></span>|<span data-ttu-id="6cdcc-225">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="6cdcc-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="6cdcc-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-226">vppTokenAccountType</span></span>|[<span data-ttu-id="6cdcc-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="6cdcc-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="6cdcc-228">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="6cdcc-229">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="6cdcc-230">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="6cdcc-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="6cdcc-231">vppTokenAppleId</span></span>|<span data-ttu-id="6cdcc-232">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-232">String</span></span>|<span data-ttu-id="6cdcc-233">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="6cdcc-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="6cdcc-234">bundleId</span></span>|<span data-ttu-id="6cdcc-235">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-235">String</span></span>|<span data-ttu-id="6cdcc-236">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-236">The Identity Name.</span></span>|
|<span data-ttu-id="6cdcc-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="6cdcc-237">vppTokenId</span></span>|<span data-ttu-id="6cdcc-238">String</span><span class="sxs-lookup"><span data-stu-id="6cdcc-238">String</span></span>|<span data-ttu-id="6cdcc-239">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="6cdcc-240">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="6cdcc-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="6cdcc-241">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6cdcc-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="6cdcc-242">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="6cdcc-243">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cdcc-243">Response</span></span>
<span data-ttu-id="6cdcc-244">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-244">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cdcc-245">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6cdcc-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cdcc-246">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6cdcc-246">Request</span></span>
<span data-ttu-id="6cdcc-247">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-247">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cdcc-248">Resposta</span><span class="sxs-lookup"><span data-stu-id="6cdcc-248">Response</span></span>
<span data-ttu-id="6cdcc-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6cdcc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





