---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a1db6319e8a318ceb735dccaafe44913348427b7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156200"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="70671-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="70671-103">Update iosStoreApp</span></span>

<span data-ttu-id="70671-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70671-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70671-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="70671-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70671-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="70671-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70671-107">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="70671-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70671-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="70671-108">Prerequisites</span></span>
<span data-ttu-id="70671-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70671-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70671-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70671-111">Permission type</span></span>|<span data-ttu-id="70671-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="70671-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70671-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70671-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70671-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70671-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70671-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70671-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70671-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70671-116">Not supported.</span></span>|
|<span data-ttu-id="70671-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70671-117">Application</span></span>|<span data-ttu-id="70671-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70671-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="70671-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70671-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="70671-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70671-120">Request headers</span></span>
|<span data-ttu-id="70671-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="70671-121">Header</span></span>|<span data-ttu-id="70671-122">Valor</span><span class="sxs-lookup"><span data-stu-id="70671-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70671-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="70671-123">Authorization</span></span>|<span data-ttu-id="70671-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70671-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70671-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="70671-125">Accept</span></span>|<span data-ttu-id="70671-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70671-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70671-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70671-127">Request body</span></span>
<span data-ttu-id="70671-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="70671-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="70671-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="70671-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="70671-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="70671-130">Property</span></span>|<span data-ttu-id="70671-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="70671-131">Type</span></span>|<span data-ttu-id="70671-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="70671-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70671-133">id</span><span class="sxs-lookup"><span data-stu-id="70671-133">id</span></span>|<span data-ttu-id="70671-134">String</span><span class="sxs-lookup"><span data-stu-id="70671-134">String</span></span>|<span data-ttu-id="70671-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="70671-135">Key of the entity.</span></span> <span data-ttu-id="70671-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-137">displayName</span><span class="sxs-lookup"><span data-stu-id="70671-137">displayName</span></span>|<span data-ttu-id="70671-138">String</span><span class="sxs-lookup"><span data-stu-id="70671-138">String</span></span>|<span data-ttu-id="70671-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="70671-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="70671-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-141">description</span><span class="sxs-lookup"><span data-stu-id="70671-141">description</span></span>|<span data-ttu-id="70671-142">String</span><span class="sxs-lookup"><span data-stu-id="70671-142">String</span></span>|<span data-ttu-id="70671-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-143">The description of the app.</span></span> <span data-ttu-id="70671-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-145">publicador</span><span class="sxs-lookup"><span data-stu-id="70671-145">publisher</span></span>|<span data-ttu-id="70671-146">String</span><span class="sxs-lookup"><span data-stu-id="70671-146">String</span></span>|<span data-ttu-id="70671-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-147">The publisher of the app.</span></span> <span data-ttu-id="70671-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="70671-149">largeIcon</span></span>|[<span data-ttu-id="70671-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="70671-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="70671-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="70671-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="70671-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70671-153">createdDateTime</span></span>|<span data-ttu-id="70671-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70671-154">DateTimeOffset</span></span>|<span data-ttu-id="70671-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-155">The date and time the app was created.</span></span> <span data-ttu-id="70671-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70671-157">lastModifiedDateTime</span></span>|<span data-ttu-id="70671-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70671-158">DateTimeOffset</span></span>|<span data-ttu-id="70671-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="70671-159">The date and time the app was last modified.</span></span> <span data-ttu-id="70671-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="70671-161">isFeatured</span></span>|<span data-ttu-id="70671-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="70671-162">Boolean</span></span>|<span data-ttu-id="70671-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="70671-164">privacyInformationUrl</span></span>|<span data-ttu-id="70671-165">String</span><span class="sxs-lookup"><span data-stu-id="70671-165">String</span></span>|<span data-ttu-id="70671-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="70671-166">The privacy statement Url.</span></span> <span data-ttu-id="70671-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="70671-168">informationUrl</span></span>|<span data-ttu-id="70671-169">String</span><span class="sxs-lookup"><span data-stu-id="70671-169">String</span></span>|<span data-ttu-id="70671-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="70671-170">The more information Url.</span></span> <span data-ttu-id="70671-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-172">owner</span><span class="sxs-lookup"><span data-stu-id="70671-172">owner</span></span>|<span data-ttu-id="70671-173">String</span><span class="sxs-lookup"><span data-stu-id="70671-173">String</span></span>|<span data-ttu-id="70671-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="70671-174">The owner of the app.</span></span> <span data-ttu-id="70671-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-176">developer</span><span class="sxs-lookup"><span data-stu-id="70671-176">developer</span></span>|<span data-ttu-id="70671-177">String</span><span class="sxs-lookup"><span data-stu-id="70671-177">String</span></span>|<span data-ttu-id="70671-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-178">The developer of the app.</span></span> <span data-ttu-id="70671-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-180">notes</span><span class="sxs-lookup"><span data-stu-id="70671-180">notes</span></span>|<span data-ttu-id="70671-181">String</span><span class="sxs-lookup"><span data-stu-id="70671-181">String</span></span>|<span data-ttu-id="70671-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-182">Notes for the app.</span></span> <span data-ttu-id="70671-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="70671-184">uploadState</span></span>|<span data-ttu-id="70671-185">Int32</span><span class="sxs-lookup"><span data-stu-id="70671-185">Int32</span></span>|<span data-ttu-id="70671-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="70671-186">The upload state.</span></span> <span data-ttu-id="70671-187">Os valores possíveis são: 0 - `Not Ready` , 1 - `Ready` , 2 - `Processing` .</span><span class="sxs-lookup"><span data-stu-id="70671-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="70671-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="70671-189">publishingState</span></span>|[<span data-ttu-id="70671-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="70671-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="70671-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="70671-191">The publishing state for the app.</span></span> <span data-ttu-id="70671-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="70671-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="70671-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="70671-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="70671-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="70671-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="70671-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="70671-195">isAssigned</span></span>|<span data-ttu-id="70671-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="70671-196">Boolean</span></span>|<span data-ttu-id="70671-197">O valor que indica se o aplicativo está atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="70671-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="70671-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="70671-199">roleScopeTagIds</span></span>|<span data-ttu-id="70671-200">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="70671-200">String collection</span></span>|<span data-ttu-id="70671-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="70671-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="70671-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="70671-203">dependentAppCount</span></span>|<span data-ttu-id="70671-204">Int32</span><span class="sxs-lookup"><span data-stu-id="70671-204">Int32</span></span>|<span data-ttu-id="70671-205">O número total de dependências que o aplicativo filho tem.</span><span class="sxs-lookup"><span data-stu-id="70671-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="70671-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="70671-207">supersedingAppCount</span></span>|<span data-ttu-id="70671-208">Int32</span><span class="sxs-lookup"><span data-stu-id="70671-208">Int32</span></span>|<span data-ttu-id="70671-209">O número total de aplicativos que este aplicativo é direta ou indiretamente é supersedido.</span><span class="sxs-lookup"><span data-stu-id="70671-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="70671-210">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="70671-211">supersededAppCount</span></span>|<span data-ttu-id="70671-212">Int32</span><span class="sxs-lookup"><span data-stu-id="70671-212">Int32</span></span>|<span data-ttu-id="70671-213">O número total de aplicativos pelos quais esse aplicativo é direta ou indiretamente sobressu valorado.</span><span class="sxs-lookup"><span data-stu-id="70671-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="70671-214">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="70671-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="70671-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="70671-215">bundleId</span></span>|<span data-ttu-id="70671-216">String</span><span class="sxs-lookup"><span data-stu-id="70671-216">String</span></span>|<span data-ttu-id="70671-217">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="70671-217">The Identity Name.</span></span>|
|<span data-ttu-id="70671-218">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="70671-218">appStoreUrl</span></span>|<span data-ttu-id="70671-219">String</span><span class="sxs-lookup"><span data-stu-id="70671-219">String</span></span>|<span data-ttu-id="70671-220">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="70671-220">The Apple App Store URL</span></span>|
|<span data-ttu-id="70671-221">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="70671-221">applicableDeviceType</span></span>|[<span data-ttu-id="70671-222">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="70671-222">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="70671-223">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="70671-223">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="70671-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="70671-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="70671-225">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="70671-225">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="70671-226">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="70671-226">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="70671-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="70671-227">Response</span></span>
<span data-ttu-id="70671-228">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70671-228">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70671-229">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70671-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="70671-230">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70671-230">Request</span></span>
<span data-ttu-id="70671-231">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="70671-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1237

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="70671-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="70671-232">Response</span></span>
<span data-ttu-id="70671-p121">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70671-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1409

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  }
}
```




