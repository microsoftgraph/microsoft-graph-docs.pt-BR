---
title: Criar iosStoreApp
description: Cria um novo objeto iosStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e56c542d8be5bc23b0dd85b57431f2bf69ae5eb0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394700"
---
# <a name="create-iosstoreapp"></a><span data-ttu-id="32020-103">Criar iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="32020-103">Create iosStoreApp</span></span>

<span data-ttu-id="32020-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32020-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32020-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32020-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32020-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32020-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32020-107">Cria um novo objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="32020-107">Create a new [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32020-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="32020-108">Prerequisites</span></span>
<span data-ttu-id="32020-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32020-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32020-111">Permission type</span></span>|<span data-ttu-id="32020-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="32020-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32020-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32020-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32020-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32020-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="32020-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32020-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32020-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32020-116">Not supported.</span></span>|
|<span data-ttu-id="32020-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32020-117">Application</span></span>|<span data-ttu-id="32020-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32020-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="32020-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32020-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="32020-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32020-120">Request headers</span></span>
|<span data-ttu-id="32020-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="32020-121">Header</span></span>|<span data-ttu-id="32020-122">Valor</span><span class="sxs-lookup"><span data-stu-id="32020-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32020-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="32020-123">Authorization</span></span>|<span data-ttu-id="32020-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="32020-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32020-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="32020-125">Accept</span></span>|<span data-ttu-id="32020-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32020-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32020-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32020-127">Request body</span></span>
<span data-ttu-id="32020-128">No corpo da solicitação, forneça uma representação JSON do objeto iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="32020-128">In the request body, supply a JSON representation for the iosStoreApp object.</span></span>

<span data-ttu-id="32020-129">A tabela a seguir mostra as propriedades obrigatórias ao criar iosStoreApp.</span><span class="sxs-lookup"><span data-stu-id="32020-129">The following table shows the properties that are required when you create the iosStoreApp.</span></span>

|<span data-ttu-id="32020-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32020-130">Property</span></span>|<span data-ttu-id="32020-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="32020-131">Type</span></span>|<span data-ttu-id="32020-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="32020-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32020-133">id</span><span class="sxs-lookup"><span data-stu-id="32020-133">id</span></span>|<span data-ttu-id="32020-134">String</span><span class="sxs-lookup"><span data-stu-id="32020-134">String</span></span>|<span data-ttu-id="32020-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="32020-135">Key of the entity.</span></span> <span data-ttu-id="32020-136">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-137">displayName</span><span class="sxs-lookup"><span data-stu-id="32020-137">displayName</span></span>|<span data-ttu-id="32020-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32020-138">String</span></span>|<span data-ttu-id="32020-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="32020-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="32020-140">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-141">description</span><span class="sxs-lookup"><span data-stu-id="32020-141">description</span></span>|<span data-ttu-id="32020-142">String</span><span class="sxs-lookup"><span data-stu-id="32020-142">String</span></span>|<span data-ttu-id="32020-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-143">The description of the app.</span></span> <span data-ttu-id="32020-144">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-145">publicador</span><span class="sxs-lookup"><span data-stu-id="32020-145">publisher</span></span>|<span data-ttu-id="32020-146">String</span><span class="sxs-lookup"><span data-stu-id="32020-146">String</span></span>|<span data-ttu-id="32020-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-147">The publisher of the app.</span></span> <span data-ttu-id="32020-148">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="32020-149">largeIcon</span></span>|[<span data-ttu-id="32020-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="32020-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="32020-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="32020-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="32020-152">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32020-153">createdDateTime</span></span>|<span data-ttu-id="32020-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32020-154">DateTimeOffset</span></span>|<span data-ttu-id="32020-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-155">The date and time the app was created.</span></span> <span data-ttu-id="32020-156">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32020-157">lastModifiedDateTime</span></span>|<span data-ttu-id="32020-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32020-158">DateTimeOffset</span></span>|<span data-ttu-id="32020-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="32020-159">The date and time the app was last modified.</span></span> <span data-ttu-id="32020-160">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="32020-161">isFeatured</span></span>|<span data-ttu-id="32020-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="32020-162">Boolean</span></span>|<span data-ttu-id="32020-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="32020-164">privacyInformationUrl</span></span>|<span data-ttu-id="32020-165">String</span><span class="sxs-lookup"><span data-stu-id="32020-165">String</span></span>|<span data-ttu-id="32020-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="32020-166">The privacy statement Url.</span></span> <span data-ttu-id="32020-167">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="32020-168">informationUrl</span></span>|<span data-ttu-id="32020-169">String</span><span class="sxs-lookup"><span data-stu-id="32020-169">String</span></span>|<span data-ttu-id="32020-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="32020-170">The more information Url.</span></span> <span data-ttu-id="32020-171">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-172">owner</span><span class="sxs-lookup"><span data-stu-id="32020-172">owner</span></span>|<span data-ttu-id="32020-173">String</span><span class="sxs-lookup"><span data-stu-id="32020-173">String</span></span>|<span data-ttu-id="32020-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="32020-174">The owner of the app.</span></span> <span data-ttu-id="32020-175">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-176">developer</span><span class="sxs-lookup"><span data-stu-id="32020-176">developer</span></span>|<span data-ttu-id="32020-177">String</span><span class="sxs-lookup"><span data-stu-id="32020-177">String</span></span>|<span data-ttu-id="32020-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-178">The developer of the app.</span></span> <span data-ttu-id="32020-179">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-180">notes</span><span class="sxs-lookup"><span data-stu-id="32020-180">notes</span></span>|<span data-ttu-id="32020-181">String</span><span class="sxs-lookup"><span data-stu-id="32020-181">String</span></span>|<span data-ttu-id="32020-182">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-182">Notes for the app.</span></span> <span data-ttu-id="32020-183">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="32020-184">uploadState</span></span>|<span data-ttu-id="32020-185">Int32</span><span class="sxs-lookup"><span data-stu-id="32020-185">Int32</span></span>|<span data-ttu-id="32020-186">O estado de upload.</span><span class="sxs-lookup"><span data-stu-id="32020-186">The upload state.</span></span> <span data-ttu-id="32020-187">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="32020-188">publishingState</span></span>|[<span data-ttu-id="32020-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="32020-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="32020-190">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32020-190">The publishing state for the app.</span></span> <span data-ttu-id="32020-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="32020-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="32020-192">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="32020-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="32020-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="32020-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="32020-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="32020-194">isAssigned</span></span>|<span data-ttu-id="32020-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="32020-195">Boolean</span></span>|<span data-ttu-id="32020-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="32020-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="32020-197">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32020-198">roleScopeTagIds</span></span>|<span data-ttu-id="32020-199">Coleção String</span><span class="sxs-lookup"><span data-stu-id="32020-199">String collection</span></span>|<span data-ttu-id="32020-200">Lista de IDs de marca de escopo para este aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="32020-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="32020-201">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="32020-202">dependentAppCount</span></span>|<span data-ttu-id="32020-203">Int32</span><span class="sxs-lookup"><span data-stu-id="32020-203">Int32</span></span>|<span data-ttu-id="32020-204">O número total de dependências do aplicativo filho.</span><span class="sxs-lookup"><span data-stu-id="32020-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="32020-205">Herdado de [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="32020-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="32020-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="32020-206">bundleId</span></span>|<span data-ttu-id="32020-207">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32020-207">String</span></span>|<span data-ttu-id="32020-208">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="32020-208">The Identity Name.</span></span>|
|<span data-ttu-id="32020-209">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="32020-209">appStoreUrl</span></span>|<span data-ttu-id="32020-210">String</span><span class="sxs-lookup"><span data-stu-id="32020-210">String</span></span>|<span data-ttu-id="32020-211">A URL da Apple App Store</span><span class="sxs-lookup"><span data-stu-id="32020-211">The Apple App Store URL</span></span>|
|<span data-ttu-id="32020-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="32020-212">applicableDeviceType</span></span>|[<span data-ttu-id="32020-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="32020-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="32020-214">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="32020-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="32020-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32020-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="32020-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="32020-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="32020-217">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="32020-217">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="32020-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="32020-218">Response</span></span>
<span data-ttu-id="32020-219">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [iosStoreApp](../resources/intune-apps-iosstoreapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32020-219">If successful, this method returns a `201 Created` response code and a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32020-220">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32020-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="32020-221">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32020-221">Request</span></span>
<span data-ttu-id="32020-222">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="32020-222">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="32020-223">Resposta</span><span class="sxs-lookup"><span data-stu-id="32020-223">Response</span></span>
<span data-ttu-id="32020-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32020-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



