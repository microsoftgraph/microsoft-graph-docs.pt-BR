---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: tfitzmac
ms.openlocfilehash: 909b19dd69e80e61370b9eed418b31eababf3d35
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351531"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="b06e0-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="b06e0-103">Update androidStoreApp</span></span>

> <span data-ttu-id="b06e0-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b06e0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b06e0-105">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b06e0-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b06e0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b06e0-106">Prerequisites</span></span>
<span data-ttu-id="b06e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b06e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b06e0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b06e0-109">Permission type</span></span>|<span data-ttu-id="b06e0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b06e0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b06e0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b06e0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b06e0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b06e0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b06e0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b06e0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b06e0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06e0-114">Not supported.</span></span>|
|<span data-ttu-id="b06e0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b06e0-115">Application</span></span>|<span data-ttu-id="b06e0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b06e0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b06e0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b06e0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b06e0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b06e0-118">Request headers</span></span>
|<span data-ttu-id="b06e0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b06e0-119">Header</span></span>|<span data-ttu-id="b06e0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b06e0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b06e0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b06e0-121">Authorization</span></span>|<span data-ttu-id="b06e0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b06e0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b06e0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b06e0-123">Accept</span></span>|<span data-ttu-id="b06e0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b06e0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b06e0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b06e0-125">Request body</span></span>
<span data-ttu-id="b06e0-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b06e0-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="b06e0-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="b06e0-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="b06e0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b06e0-128">Property</span></span>|<span data-ttu-id="b06e0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b06e0-129">Type</span></span>|<span data-ttu-id="b06e0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b06e0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b06e0-131">id</span><span class="sxs-lookup"><span data-stu-id="b06e0-131">id</span></span>|<span data-ttu-id="b06e0-132">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-132">String</span></span>|<span data-ttu-id="b06e0-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b06e0-133">Key of the entity.</span></span> <span data-ttu-id="b06e0-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b06e0-135">displayName</span></span>|<span data-ttu-id="b06e0-136">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-136">String</span></span>|<span data-ttu-id="b06e0-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b06e0-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b06e0-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-139">description</span><span class="sxs-lookup"><span data-stu-id="b06e0-139">description</span></span>|<span data-ttu-id="b06e0-140">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-140">String</span></span>|<span data-ttu-id="b06e0-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-141">The description of the app.</span></span> <span data-ttu-id="b06e0-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b06e0-143">publisher</span></span>|<span data-ttu-id="b06e0-144">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-144">String</span></span>|<span data-ttu-id="b06e0-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-145">The publisher of the app.</span></span> <span data-ttu-id="b06e0-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b06e0-147">largeIcon</span></span>|[<span data-ttu-id="b06e0-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b06e0-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b06e0-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="b06e0-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b06e0-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b06e0-151">createdDateTime</span></span>|<span data-ttu-id="b06e0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b06e0-152">DateTimeOffset</span></span>|<span data-ttu-id="b06e0-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-153">The date and time the app was created.</span></span> <span data-ttu-id="b06e0-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b06e0-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b06e0-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b06e0-156">DateTimeOffset</span></span>|<span data-ttu-id="b06e0-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b06e0-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b06e0-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b06e0-159">isFeatured</span></span>|<span data-ttu-id="b06e0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b06e0-160">Boolean</span></span>|<span data-ttu-id="b06e0-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b06e0-162">privacyInformationUrl</span></span>|<span data-ttu-id="b06e0-163">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-163">String</span></span>|<span data-ttu-id="b06e0-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="b06e0-164">The privacy statement Url.</span></span> <span data-ttu-id="b06e0-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b06e0-166">informationUrl</span></span>|<span data-ttu-id="b06e0-167">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-167">String</span></span>|<span data-ttu-id="b06e0-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="b06e0-168">The more information Url.</span></span> <span data-ttu-id="b06e0-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-170">owner</span><span class="sxs-lookup"><span data-stu-id="b06e0-170">owner</span></span>|<span data-ttu-id="b06e0-171">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-171">String</span></span>|<span data-ttu-id="b06e0-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-172">The owner of the app.</span></span> <span data-ttu-id="b06e0-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-174">developer</span><span class="sxs-lookup"><span data-stu-id="b06e0-174">developer</span></span>|<span data-ttu-id="b06e0-175">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-175">String</span></span>|<span data-ttu-id="b06e0-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-176">The developer of the app.</span></span> <span data-ttu-id="b06e0-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-178">Observações</span><span class="sxs-lookup"><span data-stu-id="b06e0-178">notes</span></span>|<span data-ttu-id="b06e0-179">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-179">String</span></span>|<span data-ttu-id="b06e0-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-180">Notes for the app.</span></span> <span data-ttu-id="b06e0-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b06e0-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b06e0-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b06e0-182">publishingState</span></span>|[<span data-ttu-id="b06e0-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b06e0-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b06e0-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b06e0-184">The publishing state for the app.</span></span> <span data-ttu-id="b06e0-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="b06e0-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b06e0-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="b06e0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b06e0-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="b06e0-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b06e0-188">packageId</span><span class="sxs-lookup"><span data-stu-id="b06e0-188">packageId</span></span>|<span data-ttu-id="b06e0-189">String</span><span class="sxs-lookup"><span data-stu-id="b06e0-189">String</span></span>|<span data-ttu-id="b06e0-190">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="b06e0-190">The package identifier.</span></span>|
|<span data-ttu-id="b06e0-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b06e0-191">appStoreUrl</span></span>|<span data-ttu-id="b06e0-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b06e0-192">String</span></span>|<span data-ttu-id="b06e0-193">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="b06e0-193">The Android app store URL.</span></span>|
|<span data-ttu-id="b06e0-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b06e0-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b06e0-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b06e0-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b06e0-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b06e0-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b06e0-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06e0-197">Response</span></span>
<span data-ttu-id="b06e0-198">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b06e0-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b06e0-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b06e0-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="b06e0-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b06e0-200">Request</span></span>
<span data-ttu-id="b06e0-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b06e0-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b06e0-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="b06e0-202">Response</span></span>
<span data-ttu-id="b06e0-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b06e0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



