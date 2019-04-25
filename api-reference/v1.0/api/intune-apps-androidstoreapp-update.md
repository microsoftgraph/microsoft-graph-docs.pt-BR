---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0408720fc5f8140e11728d7f367f738ca7636aa3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577480"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="96091-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="96091-103">Update androidStoreApp</span></span>

> <span data-ttu-id="96091-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96091-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96091-105">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="96091-105">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96091-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96091-106">Prerequisites</span></span>
<span data-ttu-id="96091-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96091-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96091-109">Permission type</span></span>|<span data-ttu-id="96091-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96091-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96091-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96091-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96091-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96091-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96091-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96091-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96091-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96091-114">Not supported.</span></span>|
|<span data-ttu-id="96091-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96091-115">Application</span></span>|<span data-ttu-id="96091-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96091-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96091-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96091-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="96091-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96091-118">Request headers</span></span>
|<span data-ttu-id="96091-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96091-119">Header</span></span>|<span data-ttu-id="96091-120">Valor</span><span class="sxs-lookup"><span data-stu-id="96091-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96091-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="96091-121">Authorization</span></span>|<span data-ttu-id="96091-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96091-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96091-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96091-123">Accept</span></span>|<span data-ttu-id="96091-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96091-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96091-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96091-125">Request body</span></span>
<span data-ttu-id="96091-126">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="96091-126">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="96091-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="96091-127">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="96091-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96091-128">Property</span></span>|<span data-ttu-id="96091-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="96091-129">Type</span></span>|<span data-ttu-id="96091-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="96091-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96091-131">id</span><span class="sxs-lookup"><span data-stu-id="96091-131">id</span></span>|<span data-ttu-id="96091-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96091-132">String</span></span>|<span data-ttu-id="96091-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96091-133">Key of the entity.</span></span> <span data-ttu-id="96091-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-135">displayName</span><span class="sxs-lookup"><span data-stu-id="96091-135">displayName</span></span>|<span data-ttu-id="96091-136">String</span><span class="sxs-lookup"><span data-stu-id="96091-136">String</span></span>|<span data-ttu-id="96091-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="96091-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="96091-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-139">description</span><span class="sxs-lookup"><span data-stu-id="96091-139">description</span></span>|<span data-ttu-id="96091-140">String</span><span class="sxs-lookup"><span data-stu-id="96091-140">String</span></span>|<span data-ttu-id="96091-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-141">The description of the app.</span></span> <span data-ttu-id="96091-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-143">publicador</span><span class="sxs-lookup"><span data-stu-id="96091-143">publisher</span></span>|<span data-ttu-id="96091-144">String</span><span class="sxs-lookup"><span data-stu-id="96091-144">String</span></span>|<span data-ttu-id="96091-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-145">The publisher of the app.</span></span> <span data-ttu-id="96091-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="96091-147">largeIcon</span></span>|[<span data-ttu-id="96091-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="96091-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="96091-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="96091-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="96091-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96091-151">createdDateTime</span></span>|<span data-ttu-id="96091-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96091-152">DateTimeOffset</span></span>|<span data-ttu-id="96091-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-153">The date and time the app was created.</span></span> <span data-ttu-id="96091-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96091-155">lastModifiedDateTime</span></span>|<span data-ttu-id="96091-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96091-156">DateTimeOffset</span></span>|<span data-ttu-id="96091-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="96091-157">The date and time the app was last modified.</span></span> <span data-ttu-id="96091-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="96091-159">isFeatured</span></span>|<span data-ttu-id="96091-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="96091-160">Boolean</span></span>|<span data-ttu-id="96091-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="96091-162">privacyInformationUrl</span></span>|<span data-ttu-id="96091-163">String</span><span class="sxs-lookup"><span data-stu-id="96091-163">String</span></span>|<span data-ttu-id="96091-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="96091-164">The privacy statement Url.</span></span> <span data-ttu-id="96091-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="96091-166">informationUrl</span></span>|<span data-ttu-id="96091-167">String</span><span class="sxs-lookup"><span data-stu-id="96091-167">String</span></span>|<span data-ttu-id="96091-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="96091-168">The more information Url.</span></span> <span data-ttu-id="96091-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-170">owner</span><span class="sxs-lookup"><span data-stu-id="96091-170">owner</span></span>|<span data-ttu-id="96091-171">String</span><span class="sxs-lookup"><span data-stu-id="96091-171">String</span></span>|<span data-ttu-id="96091-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="96091-172">The owner of the app.</span></span> <span data-ttu-id="96091-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-174">developer</span><span class="sxs-lookup"><span data-stu-id="96091-174">developer</span></span>|<span data-ttu-id="96091-175">String</span><span class="sxs-lookup"><span data-stu-id="96091-175">String</span></span>|<span data-ttu-id="96091-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-176">The developer of the app.</span></span> <span data-ttu-id="96091-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-178">notes</span><span class="sxs-lookup"><span data-stu-id="96091-178">notes</span></span>|<span data-ttu-id="96091-179">String</span><span class="sxs-lookup"><span data-stu-id="96091-179">String</span></span>|<span data-ttu-id="96091-180">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-180">Notes for the app.</span></span> <span data-ttu-id="96091-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="96091-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="96091-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="96091-182">publishingState</span></span>|[<span data-ttu-id="96091-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="96091-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="96091-184">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96091-184">The publishing state for the app.</span></span> <span data-ttu-id="96091-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="96091-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="96091-186">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="96091-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="96091-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="96091-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="96091-188">packageId</span><span class="sxs-lookup"><span data-stu-id="96091-188">packageId</span></span>|<span data-ttu-id="96091-189">String</span><span class="sxs-lookup"><span data-stu-id="96091-189">String</span></span>|<span data-ttu-id="96091-190">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="96091-190">The package identifier.</span></span>|
|<span data-ttu-id="96091-191">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="96091-191">appStoreUrl</span></span>|<span data-ttu-id="96091-192">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96091-192">String</span></span>|<span data-ttu-id="96091-193">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="96091-193">The Android app store URL.</span></span>|
|<span data-ttu-id="96091-194">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96091-194">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="96091-195">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96091-195">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="96091-196">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="96091-196">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="96091-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="96091-197">Response</span></span>
<span data-ttu-id="96091-198">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96091-198">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96091-199">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96091-199">Example</span></span>

### <a name="request"></a><span data-ttu-id="96091-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96091-200">Request</span></span>
<span data-ttu-id="96091-201">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96091-201">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96091-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="96091-202">Response</span></span>
<span data-ttu-id="96091-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96091-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



