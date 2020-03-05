---
title: Criar iosVppApp
description: Cria um novo objeto iosVppApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7fc6bc1042c856c222fb42a31a68bf296be0c9b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445622"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="9f277-103">Criar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="9f277-103">Create iosVppApp</span></span>

<span data-ttu-id="9f277-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9f277-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f277-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f277-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f277-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f277-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f277-107">Cria um novo objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f277-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f277-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f277-108">Prerequisites</span></span>
<span data-ttu-id="9f277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f277-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f277-111">Permission type</span></span>|<span data-ttu-id="9f277-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f277-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f277-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f277-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f277-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f277-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f277-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f277-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f277-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f277-116">Not supported.</span></span>|
|<span data-ttu-id="9f277-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f277-117">Application</span></span>|<span data-ttu-id="9f277-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f277-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f277-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f277-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9f277-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f277-120">Request headers</span></span>
|<span data-ttu-id="9f277-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f277-121">Header</span></span>|<span data-ttu-id="9f277-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9f277-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f277-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f277-123">Authorization</span></span>|<span data-ttu-id="9f277-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f277-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f277-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f277-125">Accept</span></span>|<span data-ttu-id="9f277-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f277-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f277-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f277-127">Request body</span></span>
<span data-ttu-id="9f277-128">No corpo da solicitação, forneça uma representação JSON do objeto iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="9f277-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="9f277-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosVppApp.</span><span class="sxs-lookup"><span data-stu-id="9f277-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="9f277-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f277-130">Property</span></span>|<span data-ttu-id="9f277-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f277-131">Type</span></span>|<span data-ttu-id="9f277-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f277-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f277-133">id</span><span class="sxs-lookup"><span data-stu-id="9f277-133">id</span></span>|<span data-ttu-id="9f277-134">String</span><span class="sxs-lookup"><span data-stu-id="9f277-134">String</span></span>|<span data-ttu-id="9f277-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9f277-135">Key of the entity.</span></span> <span data-ttu-id="9f277-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9f277-137">displayName</span></span>|<span data-ttu-id="9f277-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f277-138">String</span></span>|<span data-ttu-id="9f277-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9f277-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9f277-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-141">description</span><span class="sxs-lookup"><span data-stu-id="9f277-141">description</span></span>|<span data-ttu-id="9f277-142">String</span><span class="sxs-lookup"><span data-stu-id="9f277-142">String</span></span>|<span data-ttu-id="9f277-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-143">The description of the app.</span></span> <span data-ttu-id="9f277-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-145">publicador</span><span class="sxs-lookup"><span data-stu-id="9f277-145">publisher</span></span>|<span data-ttu-id="9f277-146">String</span><span class="sxs-lookup"><span data-stu-id="9f277-146">String</span></span>|<span data-ttu-id="9f277-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-147">The publisher of the app.</span></span> <span data-ttu-id="9f277-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9f277-149">largeIcon</span></span>|[<span data-ttu-id="9f277-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9f277-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9f277-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9f277-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9f277-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f277-153">createdDateTime</span></span>|<span data-ttu-id="9f277-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f277-154">DateTimeOffset</span></span>|<span data-ttu-id="9f277-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-155">The date and time the app was created.</span></span> <span data-ttu-id="9f277-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f277-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9f277-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f277-158">DateTimeOffset</span></span>|<span data-ttu-id="9f277-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9f277-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9f277-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9f277-161">isFeatured</span></span>|<span data-ttu-id="9f277-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f277-162">Boolean</span></span>|<span data-ttu-id="9f277-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9f277-164">privacyInformationUrl</span></span>|<span data-ttu-id="9f277-165">String</span><span class="sxs-lookup"><span data-stu-id="9f277-165">String</span></span>|<span data-ttu-id="9f277-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9f277-166">The privacy statement Url.</span></span> <span data-ttu-id="9f277-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9f277-168">informationUrl</span></span>|<span data-ttu-id="9f277-169">String</span><span class="sxs-lookup"><span data-stu-id="9f277-169">String</span></span>|<span data-ttu-id="9f277-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9f277-170">The more information Url.</span></span> <span data-ttu-id="9f277-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-172">owner</span><span class="sxs-lookup"><span data-stu-id="9f277-172">owner</span></span>|<span data-ttu-id="9f277-173">String</span><span class="sxs-lookup"><span data-stu-id="9f277-173">String</span></span>|<span data-ttu-id="9f277-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9f277-174">The owner of the app.</span></span> <span data-ttu-id="9f277-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-176">developer</span><span class="sxs-lookup"><span data-stu-id="9f277-176">developer</span></span>|<span data-ttu-id="9f277-177">String</span><span class="sxs-lookup"><span data-stu-id="9f277-177">String</span></span>|<span data-ttu-id="9f277-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-178">The developer of the app.</span></span> <span data-ttu-id="9f277-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-180">notes</span><span class="sxs-lookup"><span data-stu-id="9f277-180">notes</span></span>|<span data-ttu-id="9f277-181">String</span><span class="sxs-lookup"><span data-stu-id="9f277-181">String</span></span>|<span data-ttu-id="9f277-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-182">Notes for the app.</span></span> <span data-ttu-id="9f277-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9f277-184">uploadState</span></span>|<span data-ttu-id="9f277-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9f277-185">Int32</span></span>|<span data-ttu-id="9f277-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="9f277-186">The upload state.</span></span> <span data-ttu-id="9f277-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9f277-188">publishingState</span></span>|[<span data-ttu-id="9f277-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9f277-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9f277-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-190">The publishing state for the app.</span></span> <span data-ttu-id="9f277-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9f277-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9f277-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f277-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9f277-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9f277-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9f277-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9f277-194">isAssigned</span></span>|<span data-ttu-id="9f277-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f277-195">Boolean</span></span>|<span data-ttu-id="9f277-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="9f277-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9f277-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f277-198">roleScopeTagIds</span></span>|<span data-ttu-id="9f277-199">String collection</span><span class="sxs-lookup"><span data-stu-id="9f277-199">String collection</span></span>|<span data-ttu-id="9f277-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="9f277-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9f277-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9f277-202">dependentAppCount</span></span>|<span data-ttu-id="9f277-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9f277-203">Int32</span></span>|<span data-ttu-id="9f277-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="9f277-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9f277-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9f277-206">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9f277-206">usedLicenseCount</span></span>|<span data-ttu-id="9f277-207">Int32</span><span class="sxs-lookup"><span data-stu-id="9f277-207">Int32</span></span>|<span data-ttu-id="9f277-208">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="9f277-208">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="9f277-209">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9f277-209">totalLicenseCount</span></span>|<span data-ttu-id="9f277-210">Int32</span><span class="sxs-lookup"><span data-stu-id="9f277-210">Int32</span></span>|<span data-ttu-id="9f277-211">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="9f277-211">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="9f277-212">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="9f277-212">releaseDateTime</span></span>|<span data-ttu-id="9f277-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f277-213">DateTimeOffset</span></span>|<span data-ttu-id="9f277-214">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="9f277-214">The VPP application release date and time.</span></span>|
|<span data-ttu-id="9f277-215">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9f277-215">appStoreUrl</span></span>|<span data-ttu-id="9f277-216">String</span><span class="sxs-lookup"><span data-stu-id="9f277-216">String</span></span>|<span data-ttu-id="9f277-217">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="9f277-217">The store URL.</span></span>|
|<span data-ttu-id="9f277-218">licensingType</span><span class="sxs-lookup"><span data-stu-id="9f277-218">licensingType</span></span>|[<span data-ttu-id="9f277-219">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="9f277-219">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="9f277-220">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="9f277-220">The supported License Type.</span></span>|
|<span data-ttu-id="9f277-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="9f277-221">applicableDeviceType</span></span>|[<span data-ttu-id="9f277-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="9f277-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="9f277-223">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="9f277-223">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="9f277-224">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="9f277-224">vppTokenOrganizationName</span></span>|<span data-ttu-id="9f277-225">String</span><span class="sxs-lookup"><span data-stu-id="9f277-225">String</span></span>|<span data-ttu-id="9f277-226">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="9f277-226">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="9f277-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9f277-227">vppTokenAccountType</span></span>|[<span data-ttu-id="9f277-228">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="9f277-228">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="9f277-229">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="9f277-229">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="9f277-230">Os valores possíveis são: `business` e `education`.</span><span class="sxs-lookup"><span data-stu-id="9f277-230">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="9f277-231">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="9f277-231">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="9f277-232">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="9f277-232">vppTokenAppleId</span></span>|<span data-ttu-id="9f277-233">String</span><span class="sxs-lookup"><span data-stu-id="9f277-233">String</span></span>|<span data-ttu-id="9f277-234">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="9f277-234">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9f277-235">bundleId</span><span class="sxs-lookup"><span data-stu-id="9f277-235">bundleId</span></span>|<span data-ttu-id="9f277-236">String</span><span class="sxs-lookup"><span data-stu-id="9f277-236">String</span></span>|<span data-ttu-id="9f277-237">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9f277-237">The Identity Name.</span></span>|
|<span data-ttu-id="9f277-238">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="9f277-238">vppTokenId</span></span>|<span data-ttu-id="9f277-239">String</span><span class="sxs-lookup"><span data-stu-id="9f277-239">String</span></span>|<span data-ttu-id="9f277-240">Identificador do token VPP associado a este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-240">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="9f277-241">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="9f277-241">revokeLicenseActionResults</span></span>|<span data-ttu-id="9f277-242">coleção [iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9f277-242">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="9f277-243">Resultados da revogação de ações de licença neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f277-243">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="9f277-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f277-244">Response</span></span>
<span data-ttu-id="9f277-245">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f277-245">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f277-246">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f277-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f277-247">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f277-247">Request</span></span>
<span data-ttu-id="9f277-248">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f277-248">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f277-249">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f277-249">Response</span></span>
<span data-ttu-id="9f277-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f277-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





