---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8d5c4f171300cab0b0581d000ba57c4b13a1393
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014316"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="8e475-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="8e475-103">Create androidStoreApp</span></span>

> <span data-ttu-id="8e475-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e475-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e475-105">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e475-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e475-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8e475-106">Prerequisites</span></span>
<span data-ttu-id="8e475-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e475-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e475-109">Permission type</span></span>|<span data-ttu-id="8e475-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8e475-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e475-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e475-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8e475-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e475-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e475-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e475-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e475-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e475-114">Not supported.</span></span>|
|<span data-ttu-id="8e475-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e475-115">Application</span></span>|<span data-ttu-id="8e475-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e475-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e475-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e475-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8e475-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e475-118">Request headers</span></span>
|<span data-ttu-id="8e475-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8e475-119">Header</span></span>|<span data-ttu-id="8e475-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8e475-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e475-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e475-121">Authorization</span></span>|<span data-ttu-id="8e475-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e475-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e475-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8e475-123">Accept</span></span>|<span data-ttu-id="8e475-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8e475-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e475-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e475-125">Request body</span></span>
<span data-ttu-id="8e475-126">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8e475-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="8e475-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="8e475-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="8e475-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e475-128">Property</span></span>|<span data-ttu-id="8e475-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e475-129">Type</span></span>|<span data-ttu-id="8e475-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e475-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e475-131">id</span><span class="sxs-lookup"><span data-stu-id="8e475-131">id</span></span>|<span data-ttu-id="8e475-132">String</span><span class="sxs-lookup"><span data-stu-id="8e475-132">String</span></span>|<span data-ttu-id="8e475-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8e475-133">Key of the entity.</span></span> <span data-ttu-id="8e475-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8e475-135">displayName</span></span>|<span data-ttu-id="8e475-136">String</span><span class="sxs-lookup"><span data-stu-id="8e475-136">String</span></span>|<span data-ttu-id="8e475-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8e475-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8e475-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-139">descrição</span><span class="sxs-lookup"><span data-stu-id="8e475-139">description</span></span>|<span data-ttu-id="8e475-140">String</span><span class="sxs-lookup"><span data-stu-id="8e475-140">String</span></span>|<span data-ttu-id="8e475-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-141">The description of the app.</span></span> <span data-ttu-id="8e475-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-143">publicador</span><span class="sxs-lookup"><span data-stu-id="8e475-143">publisher</span></span>|<span data-ttu-id="8e475-144">String</span><span class="sxs-lookup"><span data-stu-id="8e475-144">String</span></span>|<span data-ttu-id="8e475-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-145">The publisher of the app.</span></span> <span data-ttu-id="8e475-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8e475-147">largeIcon</span></span>|[<span data-ttu-id="8e475-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8e475-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8e475-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="8e475-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8e475-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e475-151">createdDateTime</span></span>|<span data-ttu-id="8e475-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e475-152">DateTimeOffset</span></span>|<span data-ttu-id="8e475-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-153">The date and time the app was created.</span></span> <span data-ttu-id="8e475-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e475-155">lastModifiedDateTime</span></span>|<span data-ttu-id="8e475-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e475-156">DateTimeOffset</span></span>|<span data-ttu-id="8e475-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8e475-157">The date and time the app was last modified.</span></span> <span data-ttu-id="8e475-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8e475-159">isFeatured</span></span>|<span data-ttu-id="8e475-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e475-160">Boolean</span></span>|<span data-ttu-id="8e475-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8e475-162">privacyInformationUrl</span></span>|<span data-ttu-id="8e475-163">String</span><span class="sxs-lookup"><span data-stu-id="8e475-163">String</span></span>|<span data-ttu-id="8e475-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="8e475-164">The privacy statement Url.</span></span> <span data-ttu-id="8e475-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8e475-166">informationUrl</span></span>|<span data-ttu-id="8e475-167">String</span><span class="sxs-lookup"><span data-stu-id="8e475-167">String</span></span>|<span data-ttu-id="8e475-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8e475-168">The more information Url.</span></span> <span data-ttu-id="8e475-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-170">owner</span><span class="sxs-lookup"><span data-stu-id="8e475-170">owner</span></span>|<span data-ttu-id="8e475-171">String</span><span class="sxs-lookup"><span data-stu-id="8e475-171">String</span></span>|<span data-ttu-id="8e475-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8e475-172">The owner of the app.</span></span> <span data-ttu-id="8e475-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-174">developer</span><span class="sxs-lookup"><span data-stu-id="8e475-174">developer</span></span>|<span data-ttu-id="8e475-175">String</span><span class="sxs-lookup"><span data-stu-id="8e475-175">String</span></span>|<span data-ttu-id="8e475-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-176">The developer of the app.</span></span> <span data-ttu-id="8e475-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-178">notes</span><span class="sxs-lookup"><span data-stu-id="8e475-178">notes</span></span>|<span data-ttu-id="8e475-179">String</span><span class="sxs-lookup"><span data-stu-id="8e475-179">String</span></span>|<span data-ttu-id="8e475-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-180">Notes for the app.</span></span> <span data-ttu-id="8e475-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8e475-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e475-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="8e475-182">publishingState</span></span>|[<span data-ttu-id="8e475-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8e475-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8e475-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8e475-184">The publishing state for the app.</span></span> <span data-ttu-id="8e475-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="8e475-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8e475-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="8e475-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8e475-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="8e475-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8e475-188">packageId</span><span class="sxs-lookup"><span data-stu-id="8e475-188">packageId</span></span>|<span data-ttu-id="8e475-189">String</span><span class="sxs-lookup"><span data-stu-id="8e475-189">String</span></span>|<span data-ttu-id="8e475-190">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="8e475-190">The package identifier.</span></span>|
|<span data-ttu-id="8e475-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="8e475-191">appStoreUrl</span></span>|<span data-ttu-id="8e475-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e475-192">String</span></span>|<span data-ttu-id="8e475-193">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="8e475-193">The Android app store URL.</span></span>|
|<span data-ttu-id="8e475-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e475-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8e475-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8e475-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="8e475-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="8e475-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="8e475-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e475-197">Response</span></span>
<span data-ttu-id="8e475-198">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e475-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e475-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8e475-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e475-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e475-200">Request</span></span>
<span data-ttu-id="8e475-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e475-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e475-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e475-202">Response</span></span>
<span data-ttu-id="8e475-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e475-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



