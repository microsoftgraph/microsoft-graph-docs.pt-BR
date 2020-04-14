---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e3b67af96512faea18a8b731fd10b2bc0b6f7b5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416900"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="dac0b-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="dac0b-103">Update iosStoreApp</span></span>

<span data-ttu-id="dac0b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dac0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dac0b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dac0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dac0b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dac0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dac0b-107">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="dac0b-107">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dac0b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dac0b-108">Prerequisites</span></span>
<span data-ttu-id="dac0b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dac0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dac0b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dac0b-111">Permission type</span></span>|<span data-ttu-id="dac0b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dac0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dac0b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dac0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dac0b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac0b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dac0b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dac0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dac0b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dac0b-116">Not supported.</span></span>|
|<span data-ttu-id="dac0b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dac0b-117">Application</span></span>|<span data-ttu-id="dac0b-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dac0b-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dac0b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dac0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dac0b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dac0b-120">Request headers</span></span>
|<span data-ttu-id="dac0b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dac0b-121">Header</span></span>|<span data-ttu-id="dac0b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dac0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dac0b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dac0b-123">Authorization</span></span>|<span data-ttu-id="dac0b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dac0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dac0b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dac0b-125">Accept</span></span>|<span data-ttu-id="dac0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dac0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dac0b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dac0b-127">Request body</span></span>
<span data-ttu-id="dac0b-128">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="dac0b-128">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="dac0b-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="dac0b-129">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="dac0b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dac0b-130">Property</span></span>|<span data-ttu-id="dac0b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="dac0b-131">Type</span></span>|<span data-ttu-id="dac0b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="dac0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dac0b-133">id</span><span class="sxs-lookup"><span data-stu-id="dac0b-133">id</span></span>|<span data-ttu-id="dac0b-134">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-134">String</span></span>|<span data-ttu-id="dac0b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dac0b-135">Key of the entity.</span></span> <span data-ttu-id="dac0b-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dac0b-137">displayName</span></span>|<span data-ttu-id="dac0b-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dac0b-138">String</span></span>|<span data-ttu-id="dac0b-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="dac0b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dac0b-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-141">description</span><span class="sxs-lookup"><span data-stu-id="dac0b-141">description</span></span>|<span data-ttu-id="dac0b-142">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-142">String</span></span>|<span data-ttu-id="dac0b-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-143">The description of the app.</span></span> <span data-ttu-id="dac0b-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-145">publicador</span><span class="sxs-lookup"><span data-stu-id="dac0b-145">publisher</span></span>|<span data-ttu-id="dac0b-146">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-146">String</span></span>|<span data-ttu-id="dac0b-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-147">The publisher of the app.</span></span> <span data-ttu-id="dac0b-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dac0b-149">largeIcon</span></span>|[<span data-ttu-id="dac0b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dac0b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dac0b-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="dac0b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dac0b-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dac0b-153">createdDateTime</span></span>|<span data-ttu-id="dac0b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dac0b-154">DateTimeOffset</span></span>|<span data-ttu-id="dac0b-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-155">The date and time the app was created.</span></span> <span data-ttu-id="dac0b-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dac0b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="dac0b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dac0b-158">DateTimeOffset</span></span>|<span data-ttu-id="dac0b-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dac0b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="dac0b-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dac0b-161">isFeatured</span></span>|<span data-ttu-id="dac0b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dac0b-162">Boolean</span></span>|<span data-ttu-id="dac0b-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dac0b-164">privacyInformationUrl</span></span>|<span data-ttu-id="dac0b-165">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-165">String</span></span>|<span data-ttu-id="dac0b-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="dac0b-166">The privacy statement Url.</span></span> <span data-ttu-id="dac0b-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dac0b-168">informationUrl</span></span>|<span data-ttu-id="dac0b-169">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-169">String</span></span>|<span data-ttu-id="dac0b-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="dac0b-170">The more information Url.</span></span> <span data-ttu-id="dac0b-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-172">owner</span><span class="sxs-lookup"><span data-stu-id="dac0b-172">owner</span></span>|<span data-ttu-id="dac0b-173">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-173">String</span></span>|<span data-ttu-id="dac0b-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-174">The owner of the app.</span></span> <span data-ttu-id="dac0b-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-176">developer</span><span class="sxs-lookup"><span data-stu-id="dac0b-176">developer</span></span>|<span data-ttu-id="dac0b-177">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-177">String</span></span>|<span data-ttu-id="dac0b-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-178">The developer of the app.</span></span> <span data-ttu-id="dac0b-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-180">notes</span><span class="sxs-lookup"><span data-stu-id="dac0b-180">notes</span></span>|<span data-ttu-id="dac0b-181">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-181">String</span></span>|<span data-ttu-id="dac0b-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-182">Notes for the app.</span></span> <span data-ttu-id="dac0b-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="dac0b-184">uploadState</span></span>|<span data-ttu-id="dac0b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="dac0b-185">Int32</span></span>|<span data-ttu-id="dac0b-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="dac0b-186">The upload state.</span></span> <span data-ttu-id="dac0b-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="dac0b-188">publishingState</span></span>|[<span data-ttu-id="dac0b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dac0b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dac0b-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-190">The publishing state for the app.</span></span> <span data-ttu-id="dac0b-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="dac0b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dac0b-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="dac0b-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="dac0b-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="dac0b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dac0b-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dac0b-194">isAssigned</span></span>|<span data-ttu-id="dac0b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="dac0b-195">Boolean</span></span>|<span data-ttu-id="dac0b-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="dac0b-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dac0b-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dac0b-198">roleScopeTagIds</span></span>|<span data-ttu-id="dac0b-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dac0b-199">String collection</span></span>|<span data-ttu-id="dac0b-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="dac0b-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dac0b-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="dac0b-202">dependentAppCount</span></span>|<span data-ttu-id="dac0b-203">Int32</span><span class="sxs-lookup"><span data-stu-id="dac0b-203">Int32</span></span>|<span data-ttu-id="dac0b-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="dac0b-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dac0b-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dac0b-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="dac0b-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="dac0b-206">bundleId</span></span>|<span data-ttu-id="dac0b-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dac0b-207">String</span></span>|<span data-ttu-id="dac0b-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="dac0b-208">The Identity Name.</span></span>|
|<span data-ttu-id="dac0b-209">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dac0b-209">appStoreUrl</span></span>|<span data-ttu-id="dac0b-210">String</span><span class="sxs-lookup"><span data-stu-id="dac0b-210">String</span></span>|<span data-ttu-id="dac0b-211">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="dac0b-211">The Apple App Store URL</span></span>|
|<span data-ttu-id="dac0b-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dac0b-212">applicableDeviceType</span></span>|[<span data-ttu-id="dac0b-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dac0b-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dac0b-214">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="dac0b-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="dac0b-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dac0b-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dac0b-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dac0b-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="dac0b-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="dac0b-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="dac0b-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac0b-218">Response</span></span>
<span data-ttu-id="dac0b-219">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dac0b-219">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dac0b-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dac0b-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="dac0b-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dac0b-221">Request</span></span>
<span data-ttu-id="dac0b-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dac0b-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1160

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
    "v13_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="dac0b-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="dac0b-223">Response</span></span>
<span data-ttu-id="dac0b-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dac0b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1332

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
    "v13_0": true
  }
}
```



