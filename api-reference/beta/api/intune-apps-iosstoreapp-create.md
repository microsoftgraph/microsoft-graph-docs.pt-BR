---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db79e14bc3efdc6cc102697b980eac833f07e114
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790081"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="fe3d6-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="fe3d6-103">Create iosStoreApp</span></span>

<span data-ttu-id="fe3d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe3d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe3d6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe3d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe3d6-107">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe3d6-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe3d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fe3d6-108">Prerequisites</span></span>
<span data-ttu-id="fe3d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe3d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe3d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe3d6-111">Permission type</span></span>|<span data-ttu-id="fe3d6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe3d6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe3d6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3d6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe3d6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe3d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-116">Not supported.</span></span>|
|<span data-ttu-id="fe3d6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe3d6-117">Application</span></span>|<span data-ttu-id="fe3d6-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe3d6-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe3d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe3d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fe3d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3d6-120">Request headers</span></span>
|<span data-ttu-id="fe3d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe3d6-121">Header</span></span>|<span data-ttu-id="fe3d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fe3d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe3d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe3d6-123">Authorization</span></span>|<span data-ttu-id="fe3d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe3d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fe3d6-125">Accept</span></span>|<span data-ttu-id="fe3d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe3d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe3d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3d6-127">Request body</span></span>
<span data-ttu-id="fe3d6-128">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="fe3d6-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="fe3d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe3d6-130">Property</span></span>|<span data-ttu-id="fe3d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe3d6-131">Type</span></span>|<span data-ttu-id="fe3d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe3d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3d6-133">id</span><span class="sxs-lookup"><span data-stu-id="fe3d6-133">id</span></span>|<span data-ttu-id="fe3d6-134">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-134">String</span></span>|<span data-ttu-id="fe3d6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-135">Key of the entity.</span></span> <span data-ttu-id="fe3d6-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fe3d6-137">displayName</span></span>|<span data-ttu-id="fe3d6-138">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-138">String</span></span>|<span data-ttu-id="fe3d6-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fe3d6-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-141">description</span><span class="sxs-lookup"><span data-stu-id="fe3d6-141">description</span></span>|<span data-ttu-id="fe3d6-142">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-142">String</span></span>|<span data-ttu-id="fe3d6-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-143">The description of the app.</span></span> <span data-ttu-id="fe3d6-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-145">publicador</span><span class="sxs-lookup"><span data-stu-id="fe3d6-145">publisher</span></span>|<span data-ttu-id="fe3d6-146">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-146">String</span></span>|<span data-ttu-id="fe3d6-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-147">The publisher of the app.</span></span> <span data-ttu-id="fe3d6-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fe3d6-149">largeIcon</span></span>|[<span data-ttu-id="fe3d6-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fe3d6-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fe3d6-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fe3d6-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe3d6-153">createdDateTime</span></span>|<span data-ttu-id="fe3d6-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe3d6-154">DateTimeOffset</span></span>|<span data-ttu-id="fe3d6-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-155">The date and time the app was created.</span></span> <span data-ttu-id="fe3d6-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe3d6-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fe3d6-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe3d6-158">DateTimeOffset</span></span>|<span data-ttu-id="fe3d6-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fe3d6-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fe3d6-161">isFeatured</span></span>|<span data-ttu-id="fe3d6-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe3d6-162">Boolean</span></span>|<span data-ttu-id="fe3d6-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fe3d6-164">privacyInformationUrl</span></span>|<span data-ttu-id="fe3d6-165">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-165">String</span></span>|<span data-ttu-id="fe3d6-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-166">The privacy statement Url.</span></span> <span data-ttu-id="fe3d6-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fe3d6-168">informationUrl</span></span>|<span data-ttu-id="fe3d6-169">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-169">String</span></span>|<span data-ttu-id="fe3d6-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-170">The more information Url.</span></span> <span data-ttu-id="fe3d6-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-172">owner</span><span class="sxs-lookup"><span data-stu-id="fe3d6-172">owner</span></span>|<span data-ttu-id="fe3d6-173">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-173">String</span></span>|<span data-ttu-id="fe3d6-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-174">The owner of the app.</span></span> <span data-ttu-id="fe3d6-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-176">developer</span><span class="sxs-lookup"><span data-stu-id="fe3d6-176">developer</span></span>|<span data-ttu-id="fe3d6-177">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-177">String</span></span>|<span data-ttu-id="fe3d6-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-178">The developer of the app.</span></span> <span data-ttu-id="fe3d6-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-180">notes</span><span class="sxs-lookup"><span data-stu-id="fe3d6-180">notes</span></span>|<span data-ttu-id="fe3d6-181">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-181">String</span></span>|<span data-ttu-id="fe3d6-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-182">Notes for the app.</span></span> <span data-ttu-id="fe3d6-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fe3d6-184">uploadState</span></span>|<span data-ttu-id="fe3d6-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fe3d6-185">Int32</span></span>|<span data-ttu-id="fe3d6-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-186">The upload state.</span></span> <span data-ttu-id="fe3d6-187">Os valores possíveis são: 0- `Not Ready` , 1- `Ready` , 2- `Processing` .</span><span class="sxs-lookup"><span data-stu-id="fe3d6-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="fe3d6-188">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="fe3d6-189">publishingState</span></span>|[<span data-ttu-id="fe3d6-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fe3d6-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fe3d6-191">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-191">The publishing state for the app.</span></span> <span data-ttu-id="fe3d6-192">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fe3d6-193">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="fe3d6-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="fe3d6-194">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fe3d6-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fe3d6-195">isAssigned</span></span>|<span data-ttu-id="fe3d6-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe3d6-196">Boolean</span></span>|<span data-ttu-id="fe3d6-197">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fe3d6-198">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe3d6-199">roleScopeTagIds</span></span>|<span data-ttu-id="fe3d6-200">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe3d6-200">String collection</span></span>|<span data-ttu-id="fe3d6-201">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fe3d6-202">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="fe3d6-203">dependentAppCount</span></span>|<span data-ttu-id="fe3d6-204">Int32</span><span class="sxs-lookup"><span data-stu-id="fe3d6-204">Int32</span></span>|<span data-ttu-id="fe3d6-205">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="fe3d6-206">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe3d6-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="fe3d6-207">bundleId</span><span class="sxs-lookup"><span data-stu-id="fe3d6-207">bundleId</span></span>|<span data-ttu-id="fe3d6-208">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-208">String</span></span>|<span data-ttu-id="fe3d6-209">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-209">The Identity Name.</span></span>|
|<span data-ttu-id="fe3d6-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="fe3d6-210">appStoreUrl</span></span>|<span data-ttu-id="fe3d6-211">String</span><span class="sxs-lookup"><span data-stu-id="fe3d6-211">String</span></span>|<span data-ttu-id="fe3d6-212">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="fe3d6-212">The Apple App Store URL</span></span>|
|<span data-ttu-id="fe3d6-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="fe3d6-213">applicableDeviceType</span></span>|[<span data-ttu-id="fe3d6-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="fe3d6-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="fe3d6-215">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="fe3d6-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fe3d6-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fe3d6-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fe3d6-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="fe3d6-218">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-218">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="fe3d6-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe3d6-219">Response</span></span>
<span data-ttu-id="fe3d6-220">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-220">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe3d6-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fe3d6-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe3d6-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe3d6-222">Request</span></span>
<span data-ttu-id="fe3d6-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="fe3d6-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe3d6-224">Response</span></span>
<span data-ttu-id="fe3d6-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fe3d6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



