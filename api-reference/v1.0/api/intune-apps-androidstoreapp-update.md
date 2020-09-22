---
title: Atualizar androidStoreApp
description: Atualiza as propriedades de um objeto androidStoreApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8a6b0c39cf81c36c787982df1f178453800b90a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992311"
---
# <a name="update-androidstoreapp"></a><span data-ttu-id="e435b-103">Atualizar androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="e435b-103">Update androidStoreApp</span></span>

<span data-ttu-id="e435b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e435b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e435b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e435b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e435b-106">Atualiza as propriedades de um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e435b-106">Update the properties of a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e435b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e435b-107">Prerequisites</span></span>
<span data-ttu-id="e435b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e435b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e435b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e435b-110">Permission type</span></span>|<span data-ttu-id="e435b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e435b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e435b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e435b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e435b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e435b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e435b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e435b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e435b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e435b-115">Not supported.</span></span>|
|<span data-ttu-id="e435b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e435b-116">Application</span></span>|<span data-ttu-id="e435b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e435b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e435b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e435b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e435b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e435b-119">Request headers</span></span>
|<span data-ttu-id="e435b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e435b-120">Header</span></span>|<span data-ttu-id="e435b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e435b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e435b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e435b-122">Authorization</span></span>|<span data-ttu-id="e435b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e435b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e435b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e435b-124">Accept</span></span>|<span data-ttu-id="e435b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e435b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e435b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e435b-126">Request body</span></span>
<span data-ttu-id="e435b-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e435b-127">In the request body, supply a JSON representation for the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

<span data-ttu-id="e435b-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span><span class="sxs-lookup"><span data-stu-id="e435b-128">The following table shows the properties that are required when you create the [androidStoreApp](../resources/intune-apps-androidstoreapp.md).</span></span>

|<span data-ttu-id="e435b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e435b-129">Property</span></span>|<span data-ttu-id="e435b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e435b-130">Type</span></span>|<span data-ttu-id="e435b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e435b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e435b-132">id</span><span class="sxs-lookup"><span data-stu-id="e435b-132">id</span></span>|<span data-ttu-id="e435b-133">String</span><span class="sxs-lookup"><span data-stu-id="e435b-133">String</span></span>|<span data-ttu-id="e435b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e435b-134">Key of the entity.</span></span> <span data-ttu-id="e435b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e435b-136">displayName</span></span>|<span data-ttu-id="e435b-137">String</span><span class="sxs-lookup"><span data-stu-id="e435b-137">String</span></span>|<span data-ttu-id="e435b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="e435b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e435b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-140">description</span><span class="sxs-lookup"><span data-stu-id="e435b-140">description</span></span>|<span data-ttu-id="e435b-141">String</span><span class="sxs-lookup"><span data-stu-id="e435b-141">String</span></span>|<span data-ttu-id="e435b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-142">The description of the app.</span></span> <span data-ttu-id="e435b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="e435b-144">publisher</span></span>|<span data-ttu-id="e435b-145">String</span><span class="sxs-lookup"><span data-stu-id="e435b-145">String</span></span>|<span data-ttu-id="e435b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-146">The publisher of the app.</span></span> <span data-ttu-id="e435b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e435b-148">largeIcon</span></span>|[<span data-ttu-id="e435b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e435b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e435b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="e435b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e435b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e435b-152">createdDateTime</span></span>|<span data-ttu-id="e435b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e435b-153">DateTimeOffset</span></span>|<span data-ttu-id="e435b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-154">The date and time the app was created.</span></span> <span data-ttu-id="e435b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e435b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e435b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e435b-157">DateTimeOffset</span></span>|<span data-ttu-id="e435b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e435b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e435b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e435b-160">isFeatured</span></span>|<span data-ttu-id="e435b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e435b-161">Boolean</span></span>|<span data-ttu-id="e435b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e435b-163">privacyInformationUrl</span></span>|<span data-ttu-id="e435b-164">String</span><span class="sxs-lookup"><span data-stu-id="e435b-164">String</span></span>|<span data-ttu-id="e435b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="e435b-165">The privacy statement Url.</span></span> <span data-ttu-id="e435b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e435b-167">informationUrl</span></span>|<span data-ttu-id="e435b-168">String</span><span class="sxs-lookup"><span data-stu-id="e435b-168">String</span></span>|<span data-ttu-id="e435b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e435b-169">The more information Url.</span></span> <span data-ttu-id="e435b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="e435b-171">owner</span></span>|<span data-ttu-id="e435b-172">String</span><span class="sxs-lookup"><span data-stu-id="e435b-172">String</span></span>|<span data-ttu-id="e435b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="e435b-173">The owner of the app.</span></span> <span data-ttu-id="e435b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-175">developer</span><span class="sxs-lookup"><span data-stu-id="e435b-175">developer</span></span>|<span data-ttu-id="e435b-176">String</span><span class="sxs-lookup"><span data-stu-id="e435b-176">String</span></span>|<span data-ttu-id="e435b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-177">The developer of the app.</span></span> <span data-ttu-id="e435b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-179">notes</span><span class="sxs-lookup"><span data-stu-id="e435b-179">notes</span></span>|<span data-ttu-id="e435b-180">String</span><span class="sxs-lookup"><span data-stu-id="e435b-180">String</span></span>|<span data-ttu-id="e435b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-181">Notes for the app.</span></span> <span data-ttu-id="e435b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e435b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e435b-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="e435b-183">publishingState</span></span>|[<span data-ttu-id="e435b-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e435b-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e435b-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e435b-185">The publishing state for the app.</span></span> <span data-ttu-id="e435b-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="e435b-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e435b-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e435b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e435b-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e435b-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e435b-189">packageId</span><span class="sxs-lookup"><span data-stu-id="e435b-189">packageId</span></span>|<span data-ttu-id="e435b-190">String</span><span class="sxs-lookup"><span data-stu-id="e435b-190">String</span></span>|<span data-ttu-id="e435b-191">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="e435b-191">The package identifier.</span></span>|
|<span data-ttu-id="e435b-192">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e435b-192">appStoreUrl</span></span>|<span data-ttu-id="e435b-193">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e435b-193">String</span></span>|<span data-ttu-id="e435b-194">A URL da loja de aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="e435b-194">The Android app store URL.</span></span>|
|<span data-ttu-id="e435b-195">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e435b-195">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e435b-196">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e435b-196">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e435b-197">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="e435b-197">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="e435b-198">Resposta</span><span class="sxs-lookup"><span data-stu-id="e435b-198">Response</span></span>
<span data-ttu-id="e435b-199">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [androidStoreApp](../resources/intune-apps-androidstoreapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e435b-199">If successful, this method returns a `200 OK` response code and an updated [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e435b-200">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e435b-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="e435b-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e435b-201">Request</span></span>
<span data-ttu-id="e435b-202">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e435b-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e435b-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="e435b-203">Response</span></span>
<span data-ttu-id="e435b-p115">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e435b-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









