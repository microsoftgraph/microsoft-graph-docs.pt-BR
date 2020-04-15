---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 38954ac2ea4aad05e66405aa393e52aba14bb0d9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463185"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="44319-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="44319-103">Update androidStoreApp</span></span>

<span data-ttu-id="44319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44319-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44319-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44319-106">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="44319-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44319-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44319-107">Prerequisites</span></span>
<span data-ttu-id="44319-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44319-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44319-110">Permission type</span></span>|<span data-ttu-id="44319-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="44319-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44319-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44319-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44319-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44319-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44319-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44319-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44319-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44319-115">Not supported.</span></span>|
|<span data-ttu-id="44319-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44319-116">Application</span></span>|<span data-ttu-id="44319-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44319-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44319-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44319-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="44319-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44319-119">Request headers</span></span>
|<span data-ttu-id="44319-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44319-120">Header</span></span>|<span data-ttu-id="44319-121">Valor</span><span class="sxs-lookup"><span data-stu-id="44319-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44319-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="44319-122">Authorization</span></span>|<span data-ttu-id="44319-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44319-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44319-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44319-124">Accept</span></span>|<span data-ttu-id="44319-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44319-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44319-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44319-126">Request body</span></span>
<span data-ttu-id="44319-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="44319-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="44319-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="44319-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="44319-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44319-129">Property</span></span>|<span data-ttu-id="44319-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="44319-130">Type</span></span>|<span data-ttu-id="44319-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="44319-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44319-132">id</span><span class="sxs-lookup"><span data-stu-id="44319-132">id</span></span>|<span data-ttu-id="44319-133">String</span><span class="sxs-lookup"><span data-stu-id="44319-133">String</span></span>|<span data-ttu-id="44319-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="44319-134">Key of the entity.</span></span> <span data-ttu-id="44319-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44319-136">displayName</span></span>|<span data-ttu-id="44319-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44319-137">String</span></span>|<span data-ttu-id="44319-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="44319-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="44319-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-140">description</span><span class="sxs-lookup"><span data-stu-id="44319-140">description</span></span>|<span data-ttu-id="44319-141">String</span><span class="sxs-lookup"><span data-stu-id="44319-141">String</span></span>|<span data-ttu-id="44319-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-142">The description of the app.</span></span> <span data-ttu-id="44319-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-144">publicador</span><span class="sxs-lookup"><span data-stu-id="44319-144">publisher</span></span>|<span data-ttu-id="44319-145">String</span><span class="sxs-lookup"><span data-stu-id="44319-145">String</span></span>|<span data-ttu-id="44319-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-146">The publisher of the app.</span></span> <span data-ttu-id="44319-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="44319-148">largeIcon</span></span>|[<span data-ttu-id="44319-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="44319-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="44319-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="44319-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="44319-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44319-152">createdDateTime</span></span>|<span data-ttu-id="44319-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44319-153">DateTimeOffset</span></span>|<span data-ttu-id="44319-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-154">The date and time the app was created.</span></span> <span data-ttu-id="44319-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44319-156">lastModifiedDateTime</span></span>|<span data-ttu-id="44319-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44319-157">DateTimeOffset</span></span>|<span data-ttu-id="44319-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="44319-158">The date and time the app was last modified.</span></span> <span data-ttu-id="44319-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="44319-160">isFeatured</span></span>|<span data-ttu-id="44319-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="44319-161">Boolean</span></span>|<span data-ttu-id="44319-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="44319-163">privacyInformationUrl</span></span>|<span data-ttu-id="44319-164">String</span><span class="sxs-lookup"><span data-stu-id="44319-164">String</span></span>|<span data-ttu-id="44319-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="44319-165">The privacy statement Url.</span></span> <span data-ttu-id="44319-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="44319-167">informationUrl</span></span>|<span data-ttu-id="44319-168">String</span><span class="sxs-lookup"><span data-stu-id="44319-168">String</span></span>|<span data-ttu-id="44319-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="44319-169">The more information Url.</span></span> <span data-ttu-id="44319-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-171">owner</span><span class="sxs-lookup"><span data-stu-id="44319-171">owner</span></span>|<span data-ttu-id="44319-172">String</span><span class="sxs-lookup"><span data-stu-id="44319-172">String</span></span>|<span data-ttu-id="44319-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="44319-173">The owner of the app.</span></span> <span data-ttu-id="44319-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-175">developer</span><span class="sxs-lookup"><span data-stu-id="44319-175">developer</span></span>|<span data-ttu-id="44319-176">String</span><span class="sxs-lookup"><span data-stu-id="44319-176">String</span></span>|<span data-ttu-id="44319-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-177">The developer of the app.</span></span> <span data-ttu-id="44319-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-179">notes</span><span class="sxs-lookup"><span data-stu-id="44319-179">notes</span></span>|<span data-ttu-id="44319-180">String</span><span class="sxs-lookup"><span data-stu-id="44319-180">String</span></span>|<span data-ttu-id="44319-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-181">Notes for the app.</span></span> <span data-ttu-id="44319-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="44319-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="44319-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="44319-183">publishingState</span></span>|[<span data-ttu-id="44319-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="44319-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="44319-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44319-185">The publishing state for the app.</span></span> <span data-ttu-id="44319-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="44319-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="44319-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="44319-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="44319-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="44319-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="44319-189">packageId</span><span class="sxs-lookup"><span data-stu-id="44319-189">packageId</span></span>|<span data-ttu-id="44319-190">String</span><span class="sxs-lookup"><span data-stu-id="44319-190">String</span></span>|<span data-ttu-id="44319-191">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="44319-191">The package identifier.</span></span>|
|<span data-ttu-id="44319-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="44319-192">appStoreUrl</span></span>|<span data-ttu-id="44319-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44319-193">String</span></span>|<span data-ttu-id="44319-194">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="44319-194">The Android app store URL.</span></span>|
|<span data-ttu-id="44319-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="44319-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="44319-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="44319-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="44319-197">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="44319-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="44319-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="44319-198">Response</span></span>
<span data-ttu-id="44319-199">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44319-199">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44319-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44319-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="44319-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44319-201">Request</span></span>
<span data-ttu-id="44319-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44319-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 938

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="44319-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="44319-203">Response</span></span>
<span data-ttu-id="44319-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44319-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1110

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  }
}
```






