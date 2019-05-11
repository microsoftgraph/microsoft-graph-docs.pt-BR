---
title: Atualizar iosStoreApp
description: Atualiza as propriedades de um objeto iosStoreApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f368c05f365ddb3f1d1badf251a3ca07644540f8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33937404"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="5179a-103">Atualizar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="5179a-103">Update iosStoreApp</span></span>

> <span data-ttu-id="5179a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5179a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5179a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5179a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5179a-106">Atualiza as propriedades de um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5179a-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5179a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5179a-107">Prerequisites</span></span>
<span data-ttu-id="5179a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5179a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5179a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5179a-110">Permission type</span></span>|<span data-ttu-id="5179a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5179a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5179a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5179a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5179a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5179a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5179a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5179a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5179a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5179a-115">Not supported.</span></span>|
|<span data-ttu-id="5179a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5179a-116">Application</span></span>|<span data-ttu-id="5179a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5179a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5179a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5179a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5179a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5179a-119">Request headers</span></span>
|<span data-ttu-id="5179a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5179a-120">Header</span></span>|<span data-ttu-id="5179a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5179a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5179a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5179a-122">Authorization</span></span>|<span data-ttu-id="5179a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5179a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5179a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5179a-124">Accept</span></span>|<span data-ttu-id="5179a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5179a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5179a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5179a-126">Request body</span></span>
<span data-ttu-id="5179a-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5179a-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="5179a-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="5179a-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="5179a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5179a-129">Property</span></span>|<span data-ttu-id="5179a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5179a-130">Type</span></span>|<span data-ttu-id="5179a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5179a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5179a-132">id</span><span class="sxs-lookup"><span data-stu-id="5179a-132">id</span></span>|<span data-ttu-id="5179a-133">String</span><span class="sxs-lookup"><span data-stu-id="5179a-133">String</span></span>|<span data-ttu-id="5179a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5179a-134">Key of the entity.</span></span> <span data-ttu-id="5179a-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5179a-136">displayName</span></span>|<span data-ttu-id="5179a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-137">String</span></span>|<span data-ttu-id="5179a-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5179a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5179a-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-140">description</span><span class="sxs-lookup"><span data-stu-id="5179a-140">description</span></span>|<span data-ttu-id="5179a-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-141">String</span></span>|<span data-ttu-id="5179a-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-142">The description of the app.</span></span> <span data-ttu-id="5179a-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-144">publicador</span><span class="sxs-lookup"><span data-stu-id="5179a-144">publisher</span></span>|<span data-ttu-id="5179a-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-145">String</span></span>|<span data-ttu-id="5179a-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-146">The publisher of the app.</span></span> <span data-ttu-id="5179a-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5179a-148">largeIcon</span></span>|[<span data-ttu-id="5179a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5179a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5179a-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5179a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5179a-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5179a-152">createdDateTime</span></span>|<span data-ttu-id="5179a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5179a-153">DateTimeOffset</span></span>|<span data-ttu-id="5179a-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-154">The date and time the app was created.</span></span> <span data-ttu-id="5179a-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5179a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="5179a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5179a-157">DateTimeOffset</span></span>|<span data-ttu-id="5179a-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5179a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="5179a-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5179a-160">isFeatured</span></span>|<span data-ttu-id="5179a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5179a-161">Boolean</span></span>|<span data-ttu-id="5179a-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5179a-163">privacyInformationUrl</span></span>|<span data-ttu-id="5179a-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-164">String</span></span>|<span data-ttu-id="5179a-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5179a-165">The privacy statement Url.</span></span> <span data-ttu-id="5179a-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5179a-167">informationUrl</span></span>|<span data-ttu-id="5179a-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-168">String</span></span>|<span data-ttu-id="5179a-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5179a-169">The more information Url.</span></span> <span data-ttu-id="5179a-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-171">owner</span><span class="sxs-lookup"><span data-stu-id="5179a-171">owner</span></span>|<span data-ttu-id="5179a-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-172">String</span></span>|<span data-ttu-id="5179a-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5179a-173">The owner of the app.</span></span> <span data-ttu-id="5179a-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-175">developer</span><span class="sxs-lookup"><span data-stu-id="5179a-175">developer</span></span>|<span data-ttu-id="5179a-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-176">String</span></span>|<span data-ttu-id="5179a-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-177">The developer of the app.</span></span> <span data-ttu-id="5179a-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-179">notes</span><span class="sxs-lookup"><span data-stu-id="5179a-179">notes</span></span>|<span data-ttu-id="5179a-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-180">String</span></span>|<span data-ttu-id="5179a-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-181">Notes for the app.</span></span> <span data-ttu-id="5179a-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="5179a-183">uploadState</span></span>|<span data-ttu-id="5179a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="5179a-184">Int32</span></span>|<span data-ttu-id="5179a-185">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="5179a-185">The upload state.</span></span> <span data-ttu-id="5179a-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="5179a-187">publishingState</span></span>|[<span data-ttu-id="5179a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5179a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5179a-189">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5179a-189">The publishing state for the app.</span></span> <span data-ttu-id="5179a-190">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5179a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5179a-191">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5179a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5179a-192">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5179a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5179a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5179a-193">isAssigned</span></span>|<span data-ttu-id="5179a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="5179a-194">Boolean</span></span>|<span data-ttu-id="5179a-195">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="5179a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5179a-196">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5179a-197">roleScopeTagIds</span></span>|<span data-ttu-id="5179a-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-198">String collection</span></span>|<span data-ttu-id="5179a-199">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5179a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5179a-200">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="5179a-201">dependentAppCount</span></span>|<span data-ttu-id="5179a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="5179a-202">Int32</span></span>|<span data-ttu-id="5179a-203">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="5179a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="5179a-204">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5179a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5179a-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="5179a-205">bundleId</span></span>|<span data-ttu-id="5179a-206">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5179a-206">String</span></span>|<span data-ttu-id="5179a-207">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="5179a-207">The Identity Name.</span></span>|
|<span data-ttu-id="5179a-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="5179a-208">appStoreUrl</span></span>|<span data-ttu-id="5179a-209">String</span><span class="sxs-lookup"><span data-stu-id="5179a-209">String</span></span>|<span data-ttu-id="5179a-210">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="5179a-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="5179a-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5179a-211">applicableDeviceType</span></span>|[<span data-ttu-id="5179a-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5179a-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5179a-213">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="5179a-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5179a-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5179a-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5179a-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5179a-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5179a-216">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="5179a-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="5179a-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="5179a-217">Response</span></span>
<span data-ttu-id="5179a-218">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5179a-218">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5179a-219">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5179a-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="5179a-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5179a-220">Request</span></span>
<span data-ttu-id="5179a-221">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5179a-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1140

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
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="5179a-222">Resposta</span><span class="sxs-lookup"><span data-stu-id="5179a-222">Response</span></span>
<span data-ttu-id="5179a-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5179a-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1312

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
    "v12_0": true
  }
}
```




