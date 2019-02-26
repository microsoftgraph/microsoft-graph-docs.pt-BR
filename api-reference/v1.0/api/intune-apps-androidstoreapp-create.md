---
title: Criar androidStoreApp
description: Criar um novo objeto androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ceabaceec42dd6a4ca884af2c7e2b37c044f16a0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263830"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="e2267-103">Criar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="e2267-103">Create androidStoreApp</span></span>

> <span data-ttu-id="e2267-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2267-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2267-105">Criar um novo objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2267-105">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2267-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2267-106">Prerequisites</span></span>
<span data-ttu-id="e2267-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2267-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e2267-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2267-109">Permission type</span></span>|<span data-ttu-id="e2267-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2267-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2267-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2267-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2267-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2267-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2267-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2267-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2267-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2267-114">Not supported.</span></span>|
|<span data-ttu-id="e2267-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2267-115">Application</span></span>|<span data-ttu-id="e2267-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2267-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2267-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2267-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e2267-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2267-118">Request headers</span></span>
|<span data-ttu-id="e2267-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2267-119">Header</span></span>|<span data-ttu-id="e2267-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e2267-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2267-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2267-121">Authorization</span></span>|<span data-ttu-id="e2267-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2267-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2267-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2267-123">Accept</span></span>|<span data-ttu-id="e2267-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e2267-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2267-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2267-125">Request body</span></span>
<span data-ttu-id="e2267-126">No corpo da solicitação, forneça uma representação JSON do objeto androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="e2267-126">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="e2267-127">A tabela a seguir mostra as propriedades que são necessárias ao criar androidStoreApp.</span><span class="sxs-lookup"><span data-stu-id="e2267-127">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="e2267-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2267-128">Property</span></span>|<span data-ttu-id="e2267-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2267-129">Type</span></span>|<span data-ttu-id="e2267-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2267-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2267-131">id</span><span class="sxs-lookup"><span data-stu-id="e2267-131">id</span></span>|<span data-ttu-id="e2267-132">String</span><span class="sxs-lookup"><span data-stu-id="e2267-132">String</span></span>|<span data-ttu-id="e2267-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e2267-133">Key of the entity.</span></span> <span data-ttu-id="e2267-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e2267-135">displayName</span></span>|<span data-ttu-id="e2267-136">String</span><span class="sxs-lookup"><span data-stu-id="e2267-136">String</span></span>|<span data-ttu-id="e2267-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e2267-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e2267-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-139">description</span><span class="sxs-lookup"><span data-stu-id="e2267-139">description</span></span>|<span data-ttu-id="e2267-140">String</span><span class="sxs-lookup"><span data-stu-id="e2267-140">String</span></span>|<span data-ttu-id="e2267-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-141">The description of the app.</span></span> <span data-ttu-id="e2267-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e2267-143">publisher</span></span>|<span data-ttu-id="e2267-144">String</span><span class="sxs-lookup"><span data-stu-id="e2267-144">String</span></span>|<span data-ttu-id="e2267-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-145">The publisher of the app.</span></span> <span data-ttu-id="e2267-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e2267-147">largeIcon</span></span>|[<span data-ttu-id="e2267-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2267-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2267-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e2267-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e2267-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2267-151">createdDateTime</span></span>|<span data-ttu-id="e2267-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2267-152">DateTimeOffset</span></span>|<span data-ttu-id="e2267-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-153">The date and time the app was created.</span></span> <span data-ttu-id="e2267-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2267-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e2267-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2267-156">DateTimeOffset</span></span>|<span data-ttu-id="e2267-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e2267-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e2267-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e2267-159">isFeatured</span></span>|<span data-ttu-id="e2267-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2267-160">Boolean</span></span>|<span data-ttu-id="e2267-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2267-162">privacyInformationUrl</span></span>|<span data-ttu-id="e2267-163">String</span><span class="sxs-lookup"><span data-stu-id="e2267-163">String</span></span>|<span data-ttu-id="e2267-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e2267-164">The privacy statement Url.</span></span> <span data-ttu-id="e2267-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2267-166">informationUrl</span></span>|<span data-ttu-id="e2267-167">String</span><span class="sxs-lookup"><span data-stu-id="e2267-167">String</span></span>|<span data-ttu-id="e2267-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e2267-168">The more information Url.</span></span> <span data-ttu-id="e2267-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-170">owner</span><span class="sxs-lookup"><span data-stu-id="e2267-170">owner</span></span>|<span data-ttu-id="e2267-171">String</span><span class="sxs-lookup"><span data-stu-id="e2267-171">String</span></span>|<span data-ttu-id="e2267-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e2267-172">The owner of the app.</span></span> <span data-ttu-id="e2267-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-174">developer</span><span class="sxs-lookup"><span data-stu-id="e2267-174">developer</span></span>|<span data-ttu-id="e2267-175">String</span><span class="sxs-lookup"><span data-stu-id="e2267-175">String</span></span>|<span data-ttu-id="e2267-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-176">The developer of the app.</span></span> <span data-ttu-id="e2267-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-178">Observações</span><span class="sxs-lookup"><span data-stu-id="e2267-178">notes</span></span>|<span data-ttu-id="e2267-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e2267-179">String</span></span>|<span data-ttu-id="e2267-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-180">Notes for the app.</span></span> <span data-ttu-id="e2267-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2267-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e2267-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e2267-182">publishingState</span></span>|[<span data-ttu-id="e2267-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e2267-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e2267-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2267-184">The publishing state for the app.</span></span> <span data-ttu-id="e2267-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e2267-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e2267-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e2267-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e2267-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e2267-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e2267-188">packageId</span><span class="sxs-lookup"><span data-stu-id="e2267-188">packageId</span></span>|<span data-ttu-id="e2267-189">String</span><span class="sxs-lookup"><span data-stu-id="e2267-189">String</span></span>|<span data-ttu-id="e2267-190">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="e2267-190">The package identifier.</span></span>|
|<span data-ttu-id="e2267-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e2267-191">appStoreUrl</span></span>|<span data-ttu-id="e2267-192">String</span><span class="sxs-lookup"><span data-stu-id="e2267-192">String</span></span>|<span data-ttu-id="e2267-193">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="e2267-193">The Android app store URL.</span></span>|
|<span data-ttu-id="e2267-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2267-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e2267-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e2267-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e2267-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e2267-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e2267-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2267-197">Response</span></span>
<span data-ttu-id="e2267-198">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2267-198">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2267-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2267-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2267-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2267-200">Request</span></span>
<span data-ttu-id="e2267-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2267-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e2267-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2267-202">Response</span></span>
<span data-ttu-id="e2267-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2267-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



