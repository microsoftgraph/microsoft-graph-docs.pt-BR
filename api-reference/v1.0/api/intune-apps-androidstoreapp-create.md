---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 402d046204573e531b9934cc389fd103c0aabd52
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446551"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="db568-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="db568-103">Create androidStoreApp</span></span>

<span data-ttu-id="db568-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db568-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db568-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db568-106">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="db568-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db568-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db568-107">Prerequisites</span></span>
<span data-ttu-id="db568-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db568-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db568-110">Permission type</span></span>|<span data-ttu-id="db568-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db568-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db568-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db568-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db568-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db568-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db568-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db568-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db568-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db568-115">Not supported.</span></span>|
|<span data-ttu-id="db568-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db568-116">Application</span></span>|<span data-ttu-id="db568-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db568-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db568-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db568-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="db568-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db568-119">Request headers</span></span>
|<span data-ttu-id="db568-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db568-120">Header</span></span>|<span data-ttu-id="db568-121">Valor</span><span class="sxs-lookup"><span data-stu-id="db568-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db568-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="db568-122">Authorization</span></span>|<span data-ttu-id="db568-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db568-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db568-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db568-124">Accept</span></span>|<span data-ttu-id="db568-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db568-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db568-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db568-126">Request body</span></span>
<span data-ttu-id="db568-127">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="db568-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="db568-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="db568-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="db568-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db568-129">Property</span></span>|<span data-ttu-id="db568-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="db568-130">Type</span></span>|<span data-ttu-id="db568-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="db568-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db568-132">id</span><span class="sxs-lookup"><span data-stu-id="db568-132">id</span></span>|<span data-ttu-id="db568-133">String</span><span class="sxs-lookup"><span data-stu-id="db568-133">String</span></span>|<span data-ttu-id="db568-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="db568-134">Key of the entity.</span></span> <span data-ttu-id="db568-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-136">displayName</span><span class="sxs-lookup"><span data-stu-id="db568-136">displayName</span></span>|<span data-ttu-id="db568-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db568-137">String</span></span>|<span data-ttu-id="db568-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="db568-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="db568-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-140">description</span><span class="sxs-lookup"><span data-stu-id="db568-140">description</span></span>|<span data-ttu-id="db568-141">String</span><span class="sxs-lookup"><span data-stu-id="db568-141">String</span></span>|<span data-ttu-id="db568-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-142">The description of the app.</span></span> <span data-ttu-id="db568-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-144">publicador</span><span class="sxs-lookup"><span data-stu-id="db568-144">publisher</span></span>|<span data-ttu-id="db568-145">String</span><span class="sxs-lookup"><span data-stu-id="db568-145">String</span></span>|<span data-ttu-id="db568-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-146">The publisher of the app.</span></span> <span data-ttu-id="db568-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="db568-148">largeIcon</span></span>|[<span data-ttu-id="db568-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="db568-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="db568-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="db568-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="db568-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db568-152">createdDateTime</span></span>|<span data-ttu-id="db568-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db568-153">DateTimeOffset</span></span>|<span data-ttu-id="db568-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-154">The date and time the app was created.</span></span> <span data-ttu-id="db568-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db568-156">lastModifiedDateTime</span></span>|<span data-ttu-id="db568-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db568-157">DateTimeOffset</span></span>|<span data-ttu-id="db568-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="db568-158">The date and time the app was last modified.</span></span> <span data-ttu-id="db568-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="db568-160">isFeatured</span></span>|<span data-ttu-id="db568-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="db568-161">Boolean</span></span>|<span data-ttu-id="db568-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="db568-163">privacyInformationUrl</span></span>|<span data-ttu-id="db568-164">String</span><span class="sxs-lookup"><span data-stu-id="db568-164">String</span></span>|<span data-ttu-id="db568-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="db568-165">The privacy statement Url.</span></span> <span data-ttu-id="db568-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="db568-167">informationUrl</span></span>|<span data-ttu-id="db568-168">String</span><span class="sxs-lookup"><span data-stu-id="db568-168">String</span></span>|<span data-ttu-id="db568-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="db568-169">The more information Url.</span></span> <span data-ttu-id="db568-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-171">owner</span><span class="sxs-lookup"><span data-stu-id="db568-171">owner</span></span>|<span data-ttu-id="db568-172">String</span><span class="sxs-lookup"><span data-stu-id="db568-172">String</span></span>|<span data-ttu-id="db568-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="db568-173">The owner of the app.</span></span> <span data-ttu-id="db568-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-175">developer</span><span class="sxs-lookup"><span data-stu-id="db568-175">developer</span></span>|<span data-ttu-id="db568-176">String</span><span class="sxs-lookup"><span data-stu-id="db568-176">String</span></span>|<span data-ttu-id="db568-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-177">The developer of the app.</span></span> <span data-ttu-id="db568-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-179">notes</span><span class="sxs-lookup"><span data-stu-id="db568-179">notes</span></span>|<span data-ttu-id="db568-180">String</span><span class="sxs-lookup"><span data-stu-id="db568-180">String</span></span>|<span data-ttu-id="db568-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-181">Notes for the app.</span></span> <span data-ttu-id="db568-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db568-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db568-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="db568-183">publishingState</span></span>|[<span data-ttu-id="db568-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="db568-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="db568-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="db568-185">The publishing state for the app.</span></span> <span data-ttu-id="db568-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="db568-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="db568-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="db568-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="db568-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="db568-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="db568-189">packageId</span><span class="sxs-lookup"><span data-stu-id="db568-189">packageId</span></span>|<span data-ttu-id="db568-190">String</span><span class="sxs-lookup"><span data-stu-id="db568-190">String</span></span>|<span data-ttu-id="db568-191">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="db568-191">The package identifier.</span></span>|
|<span data-ttu-id="db568-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="db568-192">appStoreUrl</span></span>|<span data-ttu-id="db568-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db568-193">String</span></span>|<span data-ttu-id="db568-194">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="db568-194">The Android app store URL.</span></span>|
|<span data-ttu-id="db568-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db568-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="db568-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db568-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="db568-197">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="db568-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="db568-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="db568-198">Response</span></span>
<span data-ttu-id="db568-199">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db568-199">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db568-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db568-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="db568-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db568-201">Request</span></span>
<span data-ttu-id="db568-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db568-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="db568-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="db568-203">Response</span></span>
<span data-ttu-id="db568-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db568-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






